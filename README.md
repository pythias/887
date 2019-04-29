## 直播

<audio src="http://sk.cri.cn/887.m3u8" title="HitFM 直播" autoplay controls></audio>

## 互动

- 2018-11 多多生日祝福

    <audio src="assets/audios/20181109.aac" title="多多生日祝福" controls></audio>

- 2019-04 中秋离职祝福

    <audio src="assets/audios/20190417.aac" title="中秋离职祝福" controls></audio>

- 2019-04 复仇者联盟4观影团

    ![节奏当道](assets/images/20190423-3.jpg)

## 话题

<div class="category">
    <ul>
        {% for category in site.categories %}
        {% assign category_name = category[0] %}
        <li><a href="{{site.baseurl}}/{{ category[0] }}">{{ site.data.names[category_name] }}</a><span>({{ category[1].size }})</span></li>
        {% endfor %}
    </ul>
</div>