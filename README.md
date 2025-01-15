# woodwirk.github.io

## Header 2

This is some content on my repo.

[Here is some other content on a separate page.](./content-1)

# Sitemap

<!-- https://ongclement.com/blog/github-pages-indexing-directory-copy -->
{% assign doclist = site.pages | sort: 'url'  %}
<ul>
    {% for doc in doclist %}
        {% if doc.name contains '.md' or doc.name contains '.html' %}
            <li><a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.url }}</a></li>
        {% endif %}
    {% endfor %}
</ul>