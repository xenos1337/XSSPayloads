# XSSPayloads
funny xss payloads


## Random Styles
```javascript
var d = document.getElementsByTagName("div");

setInterval(function() {
    for (var i = 0; i < d.length; i++) {
        d[i].style.backgroundColor = gc();
        d[i].style.borderRadius = gs() + "px";
        d[i].style.fontSize = gs() + "rem";
        d[i].style.color = gc();
        d[i].style.border = gs() + "px solid " + gc();
        d[i].style.boxShadow = "0 0 " + gs() + "px " + gc();
        d[i].style.textShadow = "0 0 " + gs() + "px " + gc();
    }
}, 10);

function gc() {var c = "#"; for (var i = 0; i < 6; i++) { c += "0123456789ABCDEF"[Math.floor(Math.random() * 16)]; }return c;}
function gs() {return Math.floor(Math.random() * 10);}
```

```javascript
function gc(){for(var a="#",b=0;b<6;b++)a+="0123456789ABCDEF"[Math.floor(16*Math.random())];return a}function gs(){return Math.floor(10*Math.random())}var d=document.getElementsByTagName("div");setInterval(function(){for(var a=0;a<d.length;a++)d[a].style.backgroundColor=gc(),d[a].style.borderRadius=gs()+"px",d[a].style.fontSize=gs()+"rem",d[a].style.color=gc(),d[a].style.border=gs()+"px solid "+gc(),d[a].style.boxShadow="0 0 "+gs()+"px "+gc(),d[a].style.textShadow="0 0 "+gs()+"px "+gc()},10);
```

### Description
Adds random css and changes the colors, size, border, etc. <a href="https://i.imgur.com/3A0ECdw.mp4">(Click here for better preview)</a>

### Preview on YouTube
<img src="https://user-images.githubusercontent.com/66328734/213942929-ca31d77e-8063-4419-9f0b-ffa97981ae7e.png" href="https://i.imgur.com/3A0ECdw.mp4" />
