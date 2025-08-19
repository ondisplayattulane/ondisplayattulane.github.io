---
title: Programming
layout: blank
permalink: /programming/
---

{% capture timestamp %}January 1, {{site.sitedate}}{% endcapture %}
{% assign SiteYear = timestamp | date: "%Y" %}
{% assign NowYear = "now" | date: "%Y" %}

<html class="no-js" lang="en" dir="ltr">
<head>
{% include _head.html %}
</head>
<body id="the-body">


<!--
==================================================
Body
================================================== -->

<div data-sticky-container style="width: 100%" class="accentbg">
<div data-sticky data-options="marginTop:0;" data-top-anchor="the-body:top" style="width: 100%">

<div class="title-bar accentbg" data-responsive-toggle="example-menu" data-hide-for="medium" style="width: 100%">
<button class="menu-icon" type="button" data-toggle="example-menu"></button>
<div class="title-bar-title">{{ site.title }}</div>
</div>

<!--
==================================================
Top Bar
================================================== -->
<div class="top-bar accentbg" id="example-menu" style="width: 100%; background-color: #004042">
<ul class="vertical medium-horizontal dropdown menu menu-hover-lines" data-responsive-menu="accordion medium-dropdown">
<!--
==================================================
Home Link for Mobile
================================================== -->
<li class="accentbg home-nav-small">
<a href="{{ site.baseurl }}/">
Home
</a>
</li>
<!--
==================================================
Nav Loop
================================================== -->
{% for nav in site.data.navigation %}
<li class="accentbg {% if page.url == nav.url %}active{% endif %}">
{% if nav.url contains "http" %}<a href="{{ nav.url }}" target="_blank">{% else %}<a href="{{ site.baseurl }}{{ nav.url }}">{% endif %}
{{ nav.title }}<!--{{ page.url }} == {{ nav.url }}-->

</a>
</li>
{% endfor %}
</ul>
</div>

</div>
</div>

<!--default start-->


<div style="background-color: #D3EAEE; padding-bottom: .25rem; border-top, border-bottom: 3px dotted #D94f30">
<div class="grid-container">
<div class="sitetitle center">
<h4 class="center" style="margin-bottom: .25rem;">An exhibit platform for collective storytelling &amp; community archives</h4>
</div>
</div>
</div>

<div class="grid-container" markdown=1>
  
{{site.description}}

### Exhibition Program series

## Opening reception for On Display: a Twenty-First Century Salon des Refusés
**Thursday, August 28, from 5 pm to 8 pm in Stone Auditorium and Carroll Gallery**

Artist panel from 5-6 pm in Stone Auditorium with reception to follow.

## On Display Discussion and Collage Experience
**Thursday, September 4, from 5 pm to 6:30 pm in Carroll Gallery**

Join On Display curators for a gallery talk about the history of the 1863 Salon des Refusés in Paris, followed by a collage-making experience inspired by exhibited artworks and Dejeuner sur l’herbe by Édouard Manet.

## On Display Rejected Clothing and Objects Swap
**Thursday, September 11, from 3 pm to 4 pm in Carroll Gallery**

To reflect what things we value and reject, we invite the public to bring no more than 5 decent books, small furniture, purses, jewelry, or articles of clothing that they no longer use or were planning to get rid of, to participate in an organized swap.

## Rejection and Neglected Art Movements, a keynote address by Joseph R Givens
**Wednesday, September 17, from 6 pm to 8 pm in Stone Auditorium**

Celebrate the closing of On Display with Joseph R Givens, LSU researcher of underground and lowbrow art movements. Reception to follow.
