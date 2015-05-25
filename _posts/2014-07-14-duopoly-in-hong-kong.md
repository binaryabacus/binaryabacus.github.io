---
layout: post
title: "Duopoly in Hong Kong"
tagline: "Diving up Hong Kong by chain stores"
date: 2014-08-12
---

Despite being the [world's freest economy](http://www.heritage.org/index/explore) for 20 consecutive years, Hong Kong also ironically comes first in the [crony-capitalism index by the Economist](http://www.economist.com/news/international/21599041-countries-where-politically-connected-businessmen-are-most-likely-prosper-planet) by a long shot. It is perhaps no surprise to any Hong Kong citizens. If you have a chance to walk around the street of Hong Kong, you will find shopping malls everywhere filled with the same chain stores. More specifically, you will often find only 2 major brands in many of the markets.

<div class="vis-control">
    <p>Draw district lines by:</p>
    
    <div class="btn-group" data-toggle="buttons">
        <label class="btn btn-default active" data-target="vis-duopoly" data-fn="update('district')">
          <input type="radio" name="options" checked> Admin District
        </label>
        <label class="btn btn-default" data-target="vis-duopoly" data-fn="update('grocery')">
          <input type="radio" name="options"> <span class="block" style="background: #333c91"></span>ParknShop vs. <span class="block" style="background: #c9213a"></span> Wellcome
        </label>
        <label class="btn btn-default" data-target="vis-duopoly" data-fn="update('phramacy')">
          <input type="radio" name="options"> <span class="block" style="background: #fc6523"></span> Mannings vs. <span class="block" style="background: #00a0a0"></span> Watson's
        </label>
        <label class="btn btn-default" data-target="vis-duopoly" data-fn="update('coffee')">
          <input type="radio" name="options"> <span class="block" style="background: #b7010c"></span> Pacific Coffee vs. <span class="block" style="background: #006341"></span> Starbucks
        </label>
    </div>
</div>

<div class="vis">
    <iframe id="vis-duopoly" data-src="http://binaryabacus.github.io/binaryabacus-hk-duopoly/"></iframe>
</div>

The maps above shows what Hong Kong looks like if it is divided up based on where the closest chain stores are. Every chain store is represented by a black dot. The "district borders" are redrawn so that all points in a district is closest to that chain store than any others. Technically, this is a form of [Voronoi diagram](http://en.wikipedia.org/wiki/Voronoi_diagram) drawn on a map.

[ParknShop](http://www.parknshop.com/WebShop/index.do) and [Wellcome](http://www.wellcome.com.hk/wd2shop/en/html/index.html) are the biggest players in the grocery market; [Mannings](http://www.mannings.com.hk/eng/index.html) and [Watson's](http://www.watsons.com.hk/home/) are the biggest players in the pharmacy market; [Pacific Coffee](http://www.pacificcoffee.com/eng/index.php) and [Starbucks](http://www.starbucks.com.hk/) are the biggest players in the coffee shop industry.

Making this a duopoly among duopolies, all but one chain stores in the map above are majority-owned or operated by just 2 conglomerates: [Hustchison Whampoa](http://www.hutchison-whampoa.com/en/global/home.php) and [Dairy Farm](http://www.dairyfarmgroup.com/global/home.htm).

Starbucks, Wellcome and Mannings are operated or owned by Dairy Farm. ParknShop and Watson's are owned by Hustchison Whampoa. The exception is Pacific Coffee, but it is owned by China Resources which has yet another supermarket chains CR Vanguard.


{::options parse_block_html="true" /}
<div class="reference">
Data source and reference:

- Address: Homepage of various chain stores
- Latitude and longitude: Google Maps API
- Map: [2blam/HK-geojson](https://github.com/2blam/HK-geojson), [Metro Extracts](http://metro.teczno.com/#hong-kong), and OpenStreetMap
</div>
