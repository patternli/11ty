---
layout: base.njk
title: Home Page
templateEngineOverride: njk, md
---
## Hello World

I'm ❤️-ing 11ty!

{% for item in collections.news %}
### {{ item.data.title }}
{{ item.data.intro }}
{{ item.templateContent | safe }}
{% endfor %}