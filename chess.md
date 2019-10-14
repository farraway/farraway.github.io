---
layout: page
title: Chess
permalink: /chess/
---
{% assign series_set = site.categories.chess_series | map: "series" | uniq %}
<section id="posts">
    <header>
        <h2>Latest Episodes</h2>
    </header>
    <ul class="post-list">
    {% for series in series_set %}
        {% assign post = site.categories.chess_episode| where: "series",series | last %}
        {%- include post_preview.html %}
    {%- endfor -%}
    </ul>
</section>
{% assign seasons = site.posts | where: "layout","chess_series" %}
<section id="Seasons" style="clear: both;">
    <header>
        <h2>All Seasons</h2>
    </header>
    <ul class="post-list">

    {% for post in seasons %}
        {%- include post_preview.html %}
    {%- endfor -%}
    </ul>
</section>
