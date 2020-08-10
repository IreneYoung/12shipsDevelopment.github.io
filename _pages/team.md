---
layout: default
title: Team
permalink: /team
---
<style>
</style>
<div class="row team">
    <p class="head">team</p>
    <div class="members">
    {% assign members = site.data.team %}
    {% for member in members %}
    <div class="member">
        <img src="/assets/img/{{ member.avatar}}"/>
        <span class="name">{{ member.name }}</span><br/>
        <div class="title">
            {% for title in member.title %}
            <span>{{ title }}</span><br/>
            {% endfor %}
        </div>
        <div class="description">{{ member.description }}</div>
    </div>
    {% endfor %}
    </div>
</div>
<div class="row team">
    <p class="head">advisor</p>
    <div class="advisors">
    {% assign advisors = site.data.advisor %}
    {% for advisor in advisors %}
    <div class="advisor">
        <img src="/assets/img/{{ advisor.avatar}}"/>
        <span class="name">{{ advisor.name }}</span><br/>
        <div class="title">
            {% for title in advisor.title %}
            <span>{{ title }}</span><br/>
            {% endfor %}
        </div>
        <div class="description">{{ advisor.description }}</div>
    </div>
    {% endfor %}
    </div>
</div>

