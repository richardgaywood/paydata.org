---
title: "Canonical houserules"
linkTitle: "Canon"
type: docs
description: All houserules currently in use
weight: 1
draft: true
---



<section id="menu">
    <ul>
        {{ range $key, $taxonomy := .Site.Taxonomies.tags }}
        <li> {{ $key }} </li>
        <ul>
            {{ range $taxonomy.Pages }}
            <li hugo-nav="{{ .RelPermalink}}"><a href="{{ .Permalink}}"> {{ .LinkTitle }} </a> </li>
            {{ end }}
        </ul>
        {{ end }}
    </ul>
</section>


{{ partial "by-name.html" .}}

<ul>
  {{ range .Data.Pages }}
  <li>
    <a href="{{.RelPermalink}}">{{ .Title }}</a>
  </li>
  {{ end }}
</ul>

{{ $taxonomy := "tags" }} {{ with .Param $taxonomy }}
<ul>
  {{ range $index, $tag := . }} {{ with $.Site.GetPage (printf "/%s/%s"
  $taxonomy $tag) -}}
  <li>
    <a href="{{ .Permalink }}">{{ $tag | urlize }}</a>
  </li>
  {{- end -}} {{- end -}}
</ul>
{{ end }}

