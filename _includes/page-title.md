{%-comment%}如果有CATEGORY 显示在标题前{%endcomment%}
{%-unless page.slug contains '：' or page.categories.size<=1
  or page.slug contains page.categories.last-%}
  {{page.categories.last}}：
{%-endunless-%}

{{page.slug}}
