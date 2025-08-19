---
title: On Display Exhibition
layout: homepage
permalink: /
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
<img src="{{site.baseurl}}{{site.urlimg}}DigitalArc.svg" style="height: 9rem;" alt="DigitalArc Platform Logo" />
<h4 class="center" style="margin-bottom: .25rem;">An exhibit platform for collective storytelling &amp; community archives</h4>
</div>
</div>
</div>

<div class="grid-container" markdown=1>
  
### Curatorial Statement

The jury of the 1863 Paris Salon rejected two-thirds of works submitted, deciding that many were avant-garde for French academic standards. Facing rejection, artists joined forces to protest. Their demands would be answered by Emperor Napoleon III, who granted them an alternative space to display their works: the Salon des Refusés. This began a tradition to showcase artworks excluded from the canon. Today, On Display revisits the concept of rejection, exploring broader boundaries that challenge what art “deserves” to be exhibited. 

As viewership continually expands and artists break away from conventions, how do we define what is acceptable and what is not? On Display seeks to give voice to artworks that one might not expect to encounter in an exhibition space. The show’s curators called for art that was not only rejected from previous exhibitions, but also works that the artists themselves rejected, either because the materials did not conform to their vision or due to their own dissatisfaction with the outcome. On Display plays with the boundaries between traditional genres of art, once so valued by the Parisian Salons, to craft a space that fruitfully reflects the ever-expanding limits of contemporary art. 

Special thanks to the [Institute for Digital Arts and Humanities](https://idah.indiana.edu/) at Indiana University Bloomington that created the template for this website, which is now funded by the [Digital Justice Development Grant program at the American Council on Learned Societies](https://www.acls.org/recent-fellows/?program_id=40090&_project_year=2024).

Coordinated by:
- Claudia González-Díaz

Curated by:
- Camila Aguayo
- Hailee Corbin
- Aine Powers
- Maryluna Santos-Giraldo
