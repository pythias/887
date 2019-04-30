---
title: 首页
---

## 直播

<audio src="http://sk.cri.cn/887.m3u8" title="HitFM 直播" autoplay controls></audio>

## 互动

{% for story in site.stories %}
- [{{ story.date | date_to_string }} - {{ story.title }}]({{ story.url }})
{% if site.story_full %}
{% if story.audio %}
    <audio src="{{ story.audio }}" title="{{ story.title }}" controls></audio>
{% endif %}

{% if story.pictures %}
{% assign picture = story.pictures | first %}
    ![{{ picture.name }}]({{ picture.url }})
{% endif %}
{% endif %}
{% endfor %}

## 每日话题

{% for topic in site.topics %}
- [{{ topic.date | date_to_string }} - {{ topic.title }}]({{ topic.url }})
{% endfor %}

## Hit Extra

{% for extra in site.extras %}
- [{{ extra.date | date_to_string }} - {{ extra.title }}]({{ extra.url }})
{% endfor %}