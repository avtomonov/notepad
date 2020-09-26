# notepad
***
svg use
-----------------------------------
```
<svg class='svg-icon'>
    <use xlink:href="#right-quots"></use>
</svg>

<div style="display: none;">
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
      <symbol xmlns="http://www.w3.org/2000/svg" id="right-quots" width="11" height="9" viewBox="0 0 11 9"><g><g><path fill="#9e042e" d="M5.119 4.885a.459.459 0 0 1-.078.275.96.96 0 0 1-.27.229L.27 8.437a.25.25 0 0 1-.132.036.245.245 0 0 1-.252-.253V6.577a.4.4 0 0 1 .102-.288 2.08 2.08 0 0 1 .282-.24l2.112-1.417L.27 3.217a2.045 2.045 0 0 1-.282-.24.4.4 0 0 1-.102-.288V1.045A.246.246 0 0 1 .139.792.25.25 0 0 1 .27.83l4.5 3.048c.127.08.217.156.27.228a.46.46 0 0 1 .078.275zm6 0a.458.458 0 0 1-.078.275.957.957 0 0 1-.27.229l-4.5 3.048a.25.25 0 0 1-.132.036.246.246 0 0 1-.252-.253V6.577a.4.4 0 0 1 .102-.288c.067-.073.162-.152.282-.24l2.111-1.417-2.111-1.415a2.04 2.04 0 0 1-.282-.24.4.4 0 0 1-.102-.288V1.045a.247.247 0 0 1 .252-.253.25.25 0 0 1 .132.037l4.5 3.048c.127.08.217.156.27.228a.459.459 0 0 1 .078.275z"/></g></g></symbol>
    </svg>
</div>  

<style>
.svg-icon {
    display: inline-block;
    fill: currentColor;
    -webkit-transform: translateZ(0);
    transform: translateZ(0);
    shape-rendering: geometricPrecision;
    display: inline-block;
    vertical-align: middle;
    outline: none;
}
</style>    

```
***

***
клик вне элемента
-----------------------------------
```
$(document).on('click', function(e){
    if (!$(e.target).parents('.product-info__select').length && !$(e.target).hasClass('product-info__select')) {
        $('.product-info__select__drop').slideUp(300, function () {});
        $('.product-info__select').removeClass('active')
    }
})
```
***

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

