---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
author_profile: true
title: Welcome!
---

I'm a Senior Mining Engineer Student at Middle East Technical University.

I am currently working at Meta Nickel Cobalt I.C. as an intern at the Mineral Processing Facility in Manisa, Turkey. 

You can reach my works and my posts from the "Blog" directory. 

                                   *****
                      
**Hoşgeldiniz!**

Orta doğu Teknik Üniversitesi'nde son sınıf maden mühendisliği öğrencisiyim.

Şuanda Manisa, Türkiye'de Meta Nikel Kobalt A.Ş. cevher hazırlama tesisinde stajyer olarak çalışmaktayım.

Çalışmalarıma ve yazılarıma "Blog" kısmından ulaşabilirsiniz.


<!DOCTYPE html>
<html lang="{{ site.lang }}">
<head>...</head>
<body>
    ...
    <footer>
        <a class="active" href="#">{{ site.languageNames[site.lang] }}</a>
        {% for lang in site.languageNames %}
        {% if lang[0] == site.lang %} {% continue %} {% endif %}
        {% if page.namespace %}
        <a href="{% tl {{ page.namespace }} {{ lang[0] }} %}">{{ lang[1] }}</a>
        {% else %}
        <a href="{{ site.baseurl_root }}/{{ lang[0] }}/">{{ lang[1] }}</a>
        {% endif %}
        {% endfor %}
    </footer>
</body>
</html>
