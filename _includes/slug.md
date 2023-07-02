{%comment%}如果有CATEGORY 显示在标题前{%endcomment-%}
{%assign slug=post.slug%}{%assign categories=post.categories-%}

{%if slug contains'：'%}slug contains'：', {%endif-%}
{%if categories.size<=1%}categories.size<=1, {%endif-%}
{%if slug contains categories.last%}slug contains categories.last, {%endif-%}
  
{%capture category-%}
{%unless slug contains'：' or categories.size <= 1
  or slug contains categories.last -%}
  {{categories.last}}{%endunless%}{%endcapture-%}
{{category}}{%if category!=''and slug!=''%}：{%endif%}{{slug-}}
