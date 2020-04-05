---
---

<head>
<title>{{site.title}}</title>
</head>

{% assign svgs = site.static_files | where: "svg", true %}
{% for svg in svgs %}
  
# {{svg.basename}}

![{{svg.basename}}]({{svg.path}})

### PDF version

[{{svg.basename}}](/assets/results_pdf/{{svg.basename | append: ".pdf"}})

{% endfor %}
