+++
description = ""
featured_image = "/images/cropped-mbeck2-2400x1299.jpg"
title = "Careers"
[menu.main]
weight = 6

+++
Please select the seals below to check out opportunities throughout our state.

{{ $htmlTable := .Inner | markdownify }}
{{ $class := .Get 0 }}
{{ $old := "<table>" }}
{{ $new := printf "<table class=\"%s\">" $class }}
{{ $htmlTable := replace $htmlTable $old $new }}
{{ $htmlTable | safeHTML }}
  
{{<table "table table-striped table-bordered">}}
|------|------|------|
| Item 1   | Item 2   | Item 3   |
| Item 1a  | Item 2a  | Item 3a  |
{{</table>}}