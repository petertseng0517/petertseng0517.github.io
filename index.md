# 歡迎來到我的閱讀心得與筆記

請稍候，網站正在設定中。

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span style="font-size: 0.8em; color: #888;">({{ post.date | date: "%Y年%m月%d日" }})</span>
  </li>
{% endfor %}
</ul>