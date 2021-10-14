<ul>
  {% for post in site.posts limit:10 %}
  <li>
    <a href="{{ post.url | relative_url }}">
      <span> {{ post.date | date: "%F %T" }} </span> {{ post.title }}
    </a>
    {{ post.description }}
  </li>
  {% endfor %}
</ul>

<hr>

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
</form>
