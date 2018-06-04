---
layout: default
title: 'Tidy Swan | Content, Copy, Data and IA from Danny Chadburn'
published: true
---


# The cure for your content

#### I'm Danny, a freelance content consultant and copywriter from Brighton. I've honed my skills working for household name brands and digital agencies, generating billions of page views.

Enough [about me](/about), here's what I can do for you:

- **[Information Architecture](/content-information-architecture)** - putting content for big websites in a better structure
- **[Campaign Performance Analytics](/content-campaign-analytics)** - data dashboards and frameworks giving clear insight
- **[Content Marketing](/creative-content-marketing)** - planning award-winning creative campaigns for companies and agencies
- **[Headline Copywriting](/headline-copywriting)** - succinct messages for companies who need to attract attention

If any of these services take your fancy, you can [contact me](/contact) via [hello@tidyswan.com](mailto:hello@tidyswan.com) or on <a href="tel:+447720057767">07720 057767</a>.

## What else?

> **[Copy Right Now](/copy-right-now)** - Need a headline in a hurry? Place an order for quick turnaround copy that will get you out of a hole.

> **[Beers for Ideas](/beers-for-ideas)** - You buy me some beer, I'll send you an amazing content idea. Seems like a fair trade.

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
