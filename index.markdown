---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<div class="grid_container">
  {% for menu in site.data.menus %}
    <div class="menu-thumbnail">
      <h3>{{ menu.name }}</h3>
      {% assign menuPath = "menu-details/index.html?menu=" | append: menu. passName %}
      <a href={{ menuPath }}><img src="{{ menu.image }}" alt="{{ menu.image_alt }}" class="menu-image"></a>
      console.log({{ menu.image }});
    </div>
  {% endfor %}
</div>