---
layout: default
title: 
permalink: /
---
<link href="/assets/css/flexslider.css" rel="stylesheet">

<style>
.slogan {
    font-size: 20px; 
    font-weight: bold; 
    height:25px; 
    line-height: 32px; 
    font-family:Muli;
    text-align: center;
    margin-bottom: 10px;
}
.slogan1 {
    font-size: 50px; 
    font-weight: bold; 
    height:63px; 
    line-height: 80px; 
    font-family:Muli;
    text-align: center;
    margin-bottom: 10px;
}

.voyage {
    text-align: center;
}

.voyage .title {
        height:45px;
        font-size:36px;
        font-family:Muli;
        font-weight:bold;
        line-height:80px;
        color:rgba(0,0,0,1);
        margin-bottom: 30px;
        opacity:1;
}

.voyage .content {
    height: 114px;
    font-size:18px;
    font-family:Muli;
    font-weight:400;
    line-height:28px;
    color:rgba(0,0,0,1);
    margin: 100px;
    opacity:1;
}
</style>

<div class="row" style="padding-top: 40px">
    <p class="slogan">12ships will make your journey to the blockchain investment</p>
    <p class="slogan1">AS EASY AS POSSIBLE</p>
    <p class="slogan">by providing profitable and reliable mining infrastructure</p>
    <img src="/assets/img/banner.png" />
</div>
<div class="row voyage">
<center>
    <p class="title">12SHIPS'VOYAGE TO THE FUTURE</p>
    <p class="content">12Ships was launched to realize the paradigm of the Fourth Industrial Revolution through blockchain. <br/>We have developed both the high-performance hardware needed to keep the data recorded in the blockchain <br/> reliable and the software needed for its operations.This is the future that 12Ships will realize to turn this <br /> platform and service into a new business that is capable of expanding.</p>
</center>
</div>
<div class="row">
    <div class="products">
    {% assign products = site.data.product %}
    {% for product in products %}
    <div class="product">
        <img src="/assets/img/{{ product.assets }}" />
        <span class='title'>{{ product.name }}</span>
        <ul>
        {% for item in product.points %}
        <li><span class="point">{{ item }}</span></li>
        {% endfor %}
        </ul>
    </div> 
    {% endfor %}
    </div>
</div>
<div class="row news">
    <p class="title">News</p>
    <div class="flexslider">
        <ul class="slides">
        {% for post in site.posts %}
        <li class="item">
            <div class="new">
                {{ post.title }}
                <div class="btn"><a href="{{ post.url }}" >Read more</a></div>
            </div>
        </li> 
        {% endfor %}
        </ul>
    </div>
</div>

<script src="/assets/js/jquery.min.js"></script>
<script src="/assets/js/jquery.flexslider.js"></script>
<script type="text/javascript">
    $(window).load(function(){
      $('.flexslider').flexslider({
        animation: "slide",
        start: function(slider){
          $('body').removeClass('loading');
        },
        rtl: true,
        itemWidth: 365,
        itemMargin: 40,
        maxItems: 4,
        prevText: "",
        nextText: "",
      });
    });
</script>

<script src="/assets/js/jquery.easing.js"></script>
<script src="/assets/js/jquery.mousewheel.js"></script>
