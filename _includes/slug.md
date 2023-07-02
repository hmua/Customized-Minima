{%comment%}如果有CATEGORY 显示在标题前{%endcomment-%}
{%assign slug=post.slug%}{%assign category=post.categories.last%}
{%unless slug contains '：' or category==nil or slug contains category-%}
  {{category}}：{%endunless-%}

{{slug-}}
