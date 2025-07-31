+++
date = '{{ .Date }}'
draft = true
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
tags: []
slug = '{{ replace .File.ContentBaseName "-" " " | title }}'
showToc = true
+++
