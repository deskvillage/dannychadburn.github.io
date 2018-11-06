---
layout: default
title: 'Tidy Swan | Product Owner and Content Strategist | Danny Chadburn'
published: true
---


# Delivering bigger, better websites

#### I'm Danny, an agile Product Owner and experienced Content Strategist providing freelance services to businesses in the UK and beyond.

I've honed my craft with household name brands and digital agencies, launching market-leading products and generating billions of page views.

Enough [about me](/about), here's what I can do for you:

> **[Consultancy](/consultancy/)** - Specialist support and advice on [information architechture](/consultancy/content-information-architecture), [performance analytics](/consultancy/performance-analytics) and [content marketing](/consultancy/creative-content-marketing).

> **[Contracting](/contracting-cv/)** - Need a Product Owner or Content Strategist to lead your project? Take a look at my credentials.

> **[eBook Creation](/ebook-creation/)** - Get a lead magnet for your business with a unique asset. I offer a full production, publishing and promotion service.

#### Seen something of interest?

You can [contact me](/contact) via [hello@tidyswan.com](mailto:hello@tidyswan.com) or on <a href="tel:+447720057767">07720 057767</a>.

<div>
  <ul class="posts noList">
    {% for post in paginator.posts %}
      <li>
        <span class="date">{{ post.date | date: '%B %d, %Y' }}</span>
        <h3><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p>{% if post.description %}{{ post.description }}{% else %}{{ post.excerpt | strip_html }}{% endif %}</p>
      </li>
    {% endfor %}
  </ul>
  <!-- Pagination links -->
  <div class="pagination">
    {% if paginator.previous_page %}
      <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}" class="previous button__outline">Newer Posts</a> 
    {% endif %}
    {% if paginator.next_page %}
      <a href="{{ paginator.next_page_path | prepend: site.baseurl }}" class="next button__outline">Older Posts</a>
    {% endif %}
  </div>
</div>
