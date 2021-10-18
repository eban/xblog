<ul>
  {% for post in site.posts limit:10 %}
  <li>
    <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
    {{ post.excerpt }}
    &nbsp;
    <div class="f6"><div class="float-right">{{ post.date | date: "%F %T %z (%a)" }}</div></div>
    <hr/>
  </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="/xblog/feed.xml">via RSS</a></p>

<!-- SiteSearch Google -->
<form method=GET action="https://www.google.co.jp/search">
<p>
<input type=text name=q size=31 maxlength=255 value="">
<input type=hidden name=hl value="ja">
<input type=hidden name=ie value="UTF-8">
<input type=submit name=btnG value="Google 検索">
<input type=hidden name=domains value="jarp.does.notwork.org"><br>
<input type=radio name=sitesearch value=""> WWW を検索
<input type=radio name=sitesearch value="jarp.does.notwork.org" checked> jarp.does.notwork.org を検索 <br>
</p>
</form>
