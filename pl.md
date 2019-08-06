---
title: Jakub Koralewski - jcubed.me
tags: [jakub, koralewski, portfolio, github, frontend developer, backend developer, vue, typescript, nuxt, javascript, js, ts, sass, scss, python, obs, rust]
htmldesc: Jakub Koralewski to programista. Ta strona ma na celu pokazanie jego portfolio webowe, Pythonowe i info do kontaktu.
summary: >-
    Zajmuje się programowaniem. Robię stronki korzystając z nowoczesnych frameworków typu Vue oraz dziwne boty i skrypty w Pythonie. W planach mam nauczenie się backendu. W wolnym czasie lubię udawać, że jestem biznesmenem. Skontaktuj się ze mną kontakt@jcubed.me!
view_on_github: Obczaj profil na GitHubie
view_on_linkedin: Albo profil na LinkedIn
other_lang_path: ..
other_lang: gb
lang: pl
other_lang_cta: Change to English
---

# Ciekawe projekty
*Tytuły projektów to linki do repozytoriów na GitHubie!*{:.small}

&nbsp;

{% for project_hash in site.data.projects %}
{% assign project = project_hash[1] %} 


<img src="{{project.img}}" width="100" align="left" />

### <a href="{{project.links.github}}" target="_blank"> {{project.pl.title | default: project.title}} </a>

{{project.pl.description}}

{% if project.gif %} 

![]({{project.gif}}){:.video}

{% endif %}

#### Technical info:
  
{{project.pl.technical_info}}

&nbsp;
<hr/>
&nbsp;

{% endfor %}

## "Blog":

- [How to setup e-mail using a custom domain for free (Github Student Developer Pack + Namecheap + SendGrid + Gmail)](./blog/free-email.md)

&nbsp;
<hr/>
&nbsp;

# Skontaktuj się

<a href="mailto:kontakt@jcubed.me?subject=Witam%2C+tam%21&body=Jeste%C5%9B+niesamowity%21+Jak+to+zrobi%C5%82e%C5%9B%3F">kontakt@jcubed.me</a>




