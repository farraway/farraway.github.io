---
layout: page
title: Shop
permalink: /shop/
---

{% assign shop_chess = site.posts | where: "category","shop" | where: "department","chess" %}
{% assign shop_books = site.posts | where: "category","shop" | where: "department","book" %}
{% assign shop_mugs = site.posts | where: "category","shop" | where: "department","mug" %}
{% assign shop_coffee = site.posts | where: "category","shop" | where: "department","coffee" %}
{% assign shop_tea = site.posts | where: "category","shop" | where: "department","tea" %}
<style>
section.items {
    clear: both;
}
section.items section {
    margin-left: 10%;
}
</style>
<p style="font-style: Italic; text-align: center;">
As an Amazon Associate I earn from qualifying purchases.
</p>
<nav id="top">
    <ul>
        <li><a href="#chess">Chess Equipment</a></li>
        <li><a href="#books">Books</a></li>
        <li><a href="#mugs">Mugs</a></li>
        <li><a href="#coffee">Coffee</a></li>
        <li><a href="#tea">Tea</a></li>
    </ul>
</nav>
<section class="items" id="chess">
    <header>
        <h3>Chess Equipment</h3>
    </header>
    <section>
        {% for post in shop_chess %}
        {{ post.content}}
        {%- endfor -%}
        <p style="font-style: Italic;">(<a href="#top">Top</a>)</p>
    </section>
</section>
<section class="items" id="books">
    <header>
        <h3>Books</h3>
    </header>
    <section>
        {% for post in shop_books %}
        {{ post.content}}
        {%- endfor -%}
        <p style="font-style: Italic;">(<a href="#top">Top</a>)</p>
    </section>
</section>
<section class="items" id="mugs">
    <header>
        <h3>Mugs</h3>
    </header>
    <section>
        {% for post in shop_mugs %}
        {{ post.content}}
        {%- endfor -%}
        <p style="font-style: Italic;">(<a href="#top">Top</a>)</p>
    </section>
</section>
<section class="items" id="coffee">
    <header>
        <h3>Coffee</h3>
    </header>
    <section>
        {% for post in shop_coffee %}
        {{ post.content}}
        {%- endfor -%}
        <p style="font-style: Italic;">(<a href="#top">Top</a>)</p>
    </section>
</section>
<section class="items" id="tea">
    <header>
        <h3>Tea</h3>
    </header>
    <section>
        {% for post in shop_tea %}
        {{ post.content}}
        {%- endfor -%}
        <p style="font-style: Italic;">(<a href="#top">Top</a>)</p>
    </section>
</section>
