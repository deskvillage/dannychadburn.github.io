---
layout: default
title: 'Tidy Swan | Content, Copy and Much More'
published: true
---


# Content, as it should be

#### I'm Danny, a freelance copywriter and content consultant for Brighton.

But enough [about me](/about), this is what I can do for you:

- **[Headline Copywriting](/headline-copywriting)** - succinct messages for companies who need to attract attention
- **[Information Architecture](/content-information-architecture)** - putting content for big websites in a better structure
- **[Content Marketing](/creative-content-marketing)** - planning award-winning creative campaigns for companies and agencies
- **[Campaign Analytics](/content-campaign-analytics)** - data dashboards and frameworks that offer clear insight

If any of these services take your fancy, you can [contact me](/contact) via [hello@tidyswan.com](mailto:hello@tidyswan.com) or on <a href="tel:+447720057767">07720 057767</a>.

## What else?

> **[Copy Right Now](/copy-right-now)** <br />Need a headline in a hurry? Place an order for quick turnaround copy that will get you out of a hole.

> **[Beers for Ideas](/beer-for-ideas)** <br />You buy me some beer, I'll send you an amazing content idea. Seems like a fair trade.

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
