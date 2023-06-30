{%-comment%}如果有CATEGORY 显示在标题前{%endcomment%}
{%-unless post.slug contains '：' or post.categories.size<=1
  or post.slug contains post.categories.last-%}
  {{post.categories.last}}：
{%-endunless-%}

{{post.slug}}
