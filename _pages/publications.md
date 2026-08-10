---
layout: page
permalink: /publications/
title: publications
description: Publications by category in reversed chronological order.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<style>
  /* Year headings (2026, 2025, ...): a bit darker than the theme default */
  .publications h2.bibliography {
    color: var(--global-text-color-light);
  }
  /* Make award buttons stand out (same size as the other buttons) */
  .publications ol.bibliography li .links a.award.btn {
    color: #3b2d00;
    background-color: #eab308;
    border-color: #eab308;
    font-weight: 600;
  }
  .publications ol.bibliography li .links a.award.btn:hover {
    color: #3b2d00;
    background-color: #ca9a04;
    border-color: #ca9a04;
  }
  .publications ol.bibliography li .links a.award.btn::before {
    content: "\f091"; /* Font Awesome trophy */
    font: var(--fa-font-solid, normal 900 1em/1 "Font Awesome 7 Free");
    font-family: "Font Awesome 7 Free", "Font Awesome 6 Free", "FontAwesome";
    margin-right: 0.4em;
  }
</style>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h2 class="bibliography-section">International Conference Papers</h2>

{% bibliography --query @*[category=intl_conf] %}

<h2 class="bibliography-section">Journal Papers</h2>

{% bibliography --query @*[category=journal] %}

<h2 class="bibliography-section">Domestic Conference Papers</h2>

{% bibliography --query @*[category=domestic_conf] %}

<h2 class="bibliography-section">Technical Reports</h2>

{% bibliography --query @*[category=tech_report] %}

</div>
