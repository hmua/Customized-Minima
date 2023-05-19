{% # "如果有CATEGORY 显示在标题前" %}
{%-unless page.categories==empty-%}
  {{page.categories.last}}：
{%-endunless-%}

{{page.title}}
