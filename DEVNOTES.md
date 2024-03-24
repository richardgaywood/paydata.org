# Updating Hugo on Windows

```
$ scoop update
$ scoop update hugo hugo-extended
```


# Reminder of what I did with custom category taxonomy pages

Or at least, what I've tried so far, as (at time of writing) it's not working yet.

1. Define frontmatter in `paydata.org/content/categories/sprawlpedia/_index.md`

This sets the human-readable name associated with the category as well as the contents of the landing page at http://localhost:1313/sprawlpedia/

By default, this still appends the theme-default list of content below the stuff in the frontmatter.

2. Add `{{< full_taxo_contents >}}` to the file above to load a new partial

This new partial is defined in `paydata.org/layouts/shortcodes/full_taxo_contents.html`. 

3. Add stuff to `full_taxo_contents.html`

The version in this check-in has a crude example implementation.


## Rendering stuff in `full_taxo_contents.html`

This code in that partial:

```
{{ $posts := (where $.Site.Pages ".Params.title" "in" "Savage Worlds for Shadowrun players") }}
{{ range $posts }}
	{{ .Render "single" }}
{{ end }}
```
This renders an entire page (sidebars & all!) inside the page. Note the `single` partial is not the one I want, lol.


Open questions:
* How do I get rid of the theme's normal list of pages on the category tag landing page? (maybe: redefine `main`?)
* why does `docsy/layouts/blog/list.html` call `{{ partial "taxonomy_terms_article_wrapper.html" . -}}` when it's not a taxonomy?

## How the taxonomy root page is assembled from partials

Template defines four taxo partials:
* taxonomy_terms_article.html
    * `{{ partial "taxonomy_terms_article.html" (dict "context" $context "taxo" $taxo) -}}`
* taxonomy_terms_article_wrapper.html
* taxonomy_terms_cloud.html
* taxonomy_terms_clouds.html

what do these _do_? 

https://www.docsy.dev/docs/adding-content/taxonomy/

> The partial taxonomy_terms_article shows all assigned terms of an given taxonomy (partial parameter taxo) of an article respectively page (partial parameter context, most of the time the current page or context .).

> The partial taxonomy_terms_article_wrapper is a wrapper for the partial taxonomy_terms_article with the only parameter context (most of the time the current page or context .) and checks the taxonomy parameters of your project’s hugo.toml/hugo.yaml/hugo.json to loop threw all listed taxonomies in the parameter taxonomyPageHeader resp. all defined taxonomies of your page, if taxonomyPageHeader isn’t set

> The partial taxonomy_terms_cloud shows all used terms of an given taxonomy (partial parameter taxo) for your site (partial parameter context, most of the time the current page or context .) and with the parameter title as headline.

> The partial taxonomy_terms_clouds is a wrapper for the partial taxonomy_terms_cloud with the only parameter context (most of the time the current page or context .) and checks the taxonomy parameters of your project’s hugo.toml/hugo.yaml/hugo.json to loop threw all listed taxonomies in the parameter taxonomyCloud resp. all defined taxonomies of your page, if taxonomyCloud isn’t set.

# Interesting demo sites

https://gchq.github.io/stroom-docs/docs/install-guide/single-node-docker/ - has nice "plus" and "arrow" graphics in the left hand menu, and numbers in the right hand page nav


https://www.cloudwego.io/ - customised taxonomy pages eg https://www.cloudwego.io/projects/hertz/
also: https://github.com/cloudwego/cloudwego.github.io/tree/main/layouts
...actually, maybe not customised; maybe just forked from an old docsy & not updated

"projects" tax added here: https://github.com/cloudwego/cloudwego.github.io/commit/
72daecea937819d6a91ba23c66c210ffb21549dc


# Hugo stuff I keep forgetting

## Calling shortcodes with parameters

Call like this:

```
{{% thingy title="title" %}}
```

Then inside the partial/shortcode `.html` file, read into a Hugo page variable like this:

```
{{ $title := .Get "title" | default "Show Design Notes" }}
...
<h4>{{ $title }}</h4>
```
## Getting (eg) all pages from a taxonomy with a value in a page parameter

Call like this:

```
{{% thingy categoryToProcess="foo" %}}
```

Then access it like this:

```
{{ range .Site.Taxonomies.categories.Get (.Get "categoryToProcess") }}
```

Slightly weird syntax... think of it as:

- `.Site.Taxonomies.categories` is a map
- `.Site.Taxonomies.categories.foo` gets the key `foo` from the map directly
- `.Site.Taxonomies.categories.Get "foo"` is synomuous with the above, but explicitly calls the `.Get` method
- `(.Get "categoryToProcess")` is similar, but the 'naked' Get with no prefix is operating on the page context itself, which contains key/value pairs from any params that were called.

## Generating a unique ID eg for HTML elements

```
{{ $id := substr (md5 .Inner) 0 16 }}
```