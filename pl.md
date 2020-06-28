---
title: Jakub Koralewski - jcubed.me
tags: [jakub, koralewski, portfolio, github, frontend developer, backend developer, vue, typescript, nuxt, javascript, js, ts, sass, scss, python, obs, rust]
htmldesc: Jakub Koralewski - programista. Ta strona to portfolio z projektami i info do kontaktu.
summary:
    - "Jestem aspirującym programistą.
       Robię (oby) fajne stronki korzystając z frameworków typu Vue i React,
       dziwne boty i skrypty w Pythonie."
    - "Interesuję się językiem Rust i jego zastosowaniami oraz ML/AI."
    - "W wolnym czasie lubię udawać, że jestem biznesmenem.
       Skontaktuj się ze mną kontakt@jcubed.me!"
company_info: "Po ogromnym rodzaju zdobytych doświadczeń tu, w jcubed,
               zauważyliśmy, że korzystniej jest nanostrategicznie reintermediować
               niż całkowicie pochłonąć się w intuicyjny nano-mikro development.
               Tak naprawdę to jcubed stworzył pojęcie \"użytkownika\". 
               Szczycimy się nie tylko swoim zapasem popularnych, intuicyjnych funkcji,
               ale prostą administracją i szybkim supportem. 
               Stosujemy przysłowie \"Spróbuj włączyć i wyłączyć\" nie tylko do
               kolaboracji ale do naszego zapału do optymizacji. 
               Stosujemy także zasady DRY, KISS, FTBFS, FOAF, SOAP, WYSIAYG,
               WYSIWYG, WYSIWYM, WYWIWYG, YAFIYGI, YMMV 
               w naszej transparentej inkubacji Voodoo programming opierającej się 
               na architekturze
               klient-serwer używającej SOA REST Big Data on-the-cloud Agile
               do umożliwienia uczenia maszynowego w IoT. 
               Bo skoro jeśli rewolucjonizujesz przekonująco możliwe, że będziesz musiał
               udoskonalać iteracyjnie! A jeśli kolaborujesz współcałościowo możesz
               też musieć wdrażać hożo. Wyobraź sobie połączenie HTMLa i COBOLa.
               Tak zobrazujemy pojęcie dystrybucji wielokanałowej.
               Zauważyliśmy, że jeśli syntezujesz globalnie to będziesz architektował
               superwirusowo."
view_on_github: Obejrzyj profil na GitHubie
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
{% if project.video %} 

{{project.video}}

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

&nbsp;

## O mojej (nieistniejącej) firmie

&nbsp;
{{page.company_info}}
{: style="color:#666;"}



