---
title: Jakub Koralewski - jcubed.me
tags: [jakub, koralewski, portfolio, github, frontend developer, backend developer, vue, typescript, nuxt, javascript, js, ts, sass, scss, python, obs, rust]
htmldesc: Jakub Koralewski is a hobbist programmer. This site aims to present some of his web development and Python script projects and give some info to contact him.
summary: >-
    I am a hobbist programmer located in Poland. I (try to) develop: cool websites using modern frameworks like Vue, weird Python bots and scripts. My next goal is to learn to develop backends. In my free time I like to pretend that I own a company. Contact me at contact@jcubed.me.
view_on_github: View my profile on GitHub
other_lang: pl
lang: en
other_lang_cta: Zmień na język polski
---

# Cool projects
*Titles of the projects are links to the repositories on GitHub!*{:.small}

&nbsp;

{% for project_hash in site.data.projects %}
{% assign project = project_hash[1] %} 


<img src="{{project.img}}" width="100" align="left" />

### <a href="{{project.links.github}}" target="_blank"> {{project.title}} </a>

{{project.en.description}}

{% if project.gif %} 

![]({{project.gif}}){:.video}

{% endif %}

#### Technical info:
  
{{project.en.technical_info}}

&nbsp;
<hr/>
&nbsp;

{% endfor %}

<h2 itemscope itemtype="https://schema.org/Blog"> "Blog": </h2>

- [How to setup e-mail using a custom domain for free (Github Student Developer Pack + Namecheap + SendGrid + Gmail)](./blog/free-email.md){:itemscope="" itemtype="https://schema.org/blogPost"}

&nbsp;
<hr/>
&nbsp;

# Contact me

<a href="mailto:contact@jcubed.me?subject=Hello%2C+there%21&body=How+are+you+so+amazing%3F">contact@jcubed.me</a>

