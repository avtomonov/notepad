# notepad
***
кеширование по обновлениею категории
-----------------------------------
{% cache collections.last_updated_at %}
{% endcache %}
***

***
оставить полосу скролла фансибокс
-----------------------------------
$.fancybox.defaults.hideScrollbar = false;
***

***
создать пронумерованные по порядку элементы в emmet
-----------------------------------
.row>.cell-12*8>.count-circle{$}+.pay-online__text 
***

***
выключить shop bundle 
-----------------------------------
"not_need_shop_bundle": true,  
settings_data.json  
***

***
предподгрузка шрифтов чтобы не скакали 
-----------------------------------
```
<link rel="preload" href="{{ 'Geometria.woff' | asset_url }}" as="font" type="font/woff2" crossorigin="">  
```
***

