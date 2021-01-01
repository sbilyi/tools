#formulas
Формула Миффлина — Джеора
```python
ccal = 5 + (10* w) + (6.25*h) - (5*age)
```
https://ru.wikipedia.org/wiki/Индекс_массы_тела
```python
I = w/pow(0.01*h, 2)
```

# tools

Export youtube watchlist as csv: 
```js
var jq = document.createElement('script');
jq.src = "https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js";
document.getElementsByTagName('head')[0].appendChild(jq);
// ... give time for script to load, then type (or see below for non wait option)
setTimeout(function(){
jQuery.noConflict();
 var content;
 var resultingCSV ;
 content = jQuery('#content div.ytd-playlist-video-renderer > a')
.map(function(){
  return "\"" + jQuery(this).find("#video-title").text().trim() + "\",\"\"," + "youtube.com" + jQuery(this).attr("href");
})
resultingCSV = "";
for(i = 0; i < content.length; i++) {resultingCSV = resultingCSV.concat(content[i] + "\r\n");}
console.log(resultingCSV);
}, 1500)


```
