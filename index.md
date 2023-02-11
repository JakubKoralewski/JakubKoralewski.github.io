---
title: Jakub Koralewski - jcubed.me
tags: [jakub, koralewski, portfolio, github, frontend developer, backend developer, vue, typescript, nuxt, javascript, js, ts, sass, scss, python, obs, rust]
htmldesc: Jakub Koralewski is a hobbist programmer. This site aims to present some of his web development and Python script projects and give some info to contact him.
summary:
    - "I am a programmer located in Poland.
       I develop: (I think) cool websites
       using modern frameworks like Vue and React, weird Python
       bots, scripts and more."
    - "I'm interested in the Rust programming language and ML/AI."
    - "In my free time I like to pretend that
       I own a company.
       Contact me at contact@jcubed.me."
company_info: "After our enormous experience, we here at jcubed
               have come to know that it
               is preferable to reintermediate nano-strategically than to
               embrace nano-micro-intuitively.
               It was jcubed which first coined the term \"user\".
               We put the proverb \"Try turning it off and on again\"
               into action not only for our synergies but also for
               our power to optimize.
               We also employ the spells of DRY, KISS, FTBFS, FOAF
               SOAP, WYSIAYG, WYSIWYG, WYSIWYM, WYWIWYWYWY, FAFIYGI, YYMVV
               not only for our transparent incubation of Voodoo programming
               backed by our client-server architecture using the SOA REST
               Big Data on-the-cloud Agile for Machine Learning on IoT deives,
               but also for rewriting it in Rust.
               If 'tain't already, your budget for growing should be at
               least one-third of your budget for engineering.
               If you revolutionize compellingly, you may have to streamline iteratively.
               But then also if you synergize mega-holistically, you may have to facilitate robustly.
               But then, do you have a scheme to become user-defined?
               If not, imagine a combination of HTML and COBOL.
               That's how we will visualize the term \"bricks-and-clicks\"!
               But of course, we have also come to know that if you iterate globally then you may also architect
               super-ultra-mega-virally."
view_on_github: View my profile on GitHub
view_on_linkedin: Or my profile on LinkedIn
view_on_stackoverflow: I fix others' bugs when I'm not busy fixing mine
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

{% if project.video %}

{{project.video}}

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

&nbsp;

## About my (non-existent) company

&nbsp;
{{page.company_info}}
{:style="color:#666;"}
