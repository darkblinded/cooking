---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
# Willkommen

auf meinem Rezept Log.  Hier sammle ich alles, von dem ich glaube,
dass andere davon profitieren können. Ich stelle alles Wissen gemeinfrei zur
Verfügung - Nehmt es und macht diese Welt damit zu einem besseren/leckereren
Ort!

<div class="recipes xs-px1 xs-mt2">
  <ul>
    {% assign sorted = site.recipes | sort:"date" %}
    {% for post in sorted %}

      <li>
          <a class="block relative bg-blue" href="{{ post.url | prepend: site.baseurl }}">
            {{ post.title }}
          </a>
      </li>
    {% endfor %}
  </ul>
</div>
