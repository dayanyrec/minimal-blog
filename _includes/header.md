<header class="masthead">
  <h1 class="masthead-title">
    <a href="{{ site.baseurl }}/">{{ site.title }}<span>'s blog</span></a>
  </h1>
  <nav class="masthead-nav">
    {% for page in site.pages %}
      <a href="{{ site.baseurl | append: page.url }}">{{ page.title }}</a>
    {% endfor %}
  </nav>
</header>
