---
title: {{ $term := index ( split .File.Dir "/") 1 }}"{{ replace $term "-" " " | title }}"
description: "This is the description for {{ $term | title }}"
website: "http://{{ $term }}.com"
logo: "img/{{  $term }}.jpg"
date: {{ .Date }}
draft: false
---