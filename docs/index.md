---
title: Welcome!
layout: default
use-leaflet: true
---

<section class="flex justify-center">
  <article class="standout-box blue large">
    <div class="big-text header" id="map-box" data-aos="fade-left">
      Election Day
      {% if site.election_over %}
        <strong>was</strong>
      {% else %}
        is
      {% endif %}
      {{ site.election_date | date: "%B %d, %Y" }}.
    </div>
    <div data-aos="fade-left">
    {% comment %}
    Use this site for information about the election, and the
    candidates asking for your vote!
    {% endcomment %}
    </div>
    <div class="countdown-container" style="font-size: 1.5rem; margin-bottom: 48px;" data-aos="fade-left">
      <div class="countdown-days">
      </div>
    <!--Today is Election Day-->
    </div>
    <hr />
    <p>
      The Waterloo Region Votes team has not collected the nominee information for
      this election, but the below links list all of the canadiates who are running
      in the Region:
    </p>
    <ul>
      <li>
        <a href="https://www.cbc.ca/news/canada/kitchener-waterloo/federal-election-candidates-waterloo-region-guelph-wellington-1.7486384">
          CBC federal candidates in Waterloo Region, Guelph and Wellington County
        </a>
      </li>
      <li>
        <a href="https://poliblog.jonkman.ca/Poliblog-Elections/2025-Federal-Election/index.html">
          Bob Jonkman's federal candidate links for Waterloo Region and Brantford-Brant South-Six Nations
        </a>
      </li>
      <li>
        <a href="https://www.elections.ca/home.aspx">
          Elections Canada
        </a>
      </li>
    </ul>

    <!--
    <div class="content" data-aos="fade-up">
     <p>
     Type your address to identify your riding, or click your
     location on the map.
     </p>
     <div id="map-searchbar"></div>
     <div id="map"></div>
     <p><strong>Note:</strong> The map loads more slowly than the rest
     of the page, so be patient, or use the <a href="/ridings/">Riding listing</a>.</p>
    </div>
    -->
  </article>
</section>

<script src="{{ site.baseurl }}/assets/js/leaflet.js"></script>
<script src="{{ site.baseurl }}/assets/js/leaflet-search.min.js"></script>
<!-- This has too many dependencies to load locally. -->
<script src="https://unpkg.com/leaflet-pip@1.1.0/leaflet-pip.js"></script>
<script src="{{ site.baseurl }}/assets/js/jquery-3.6.0.min.js"></script>
<script src="{{ site.baseurl }}/assets/js/show-map.js"></script>
