---
name: js使用范例
---

# js使用范例

```
<script type="text/javascript"> 
window.onload = function(){ 
$.ajax({
url: "http://print.moe/api?limit=1&page=1&days=10&desc=1&order=0&w_max=3500&w_min=1200",
type: "POST",
dataType:'jsonp',
success:function (msg) {
                    //数据成功返回时执行次回调函数
　　　　var ul = document.getElementById('i');

　　　　//添加 li
　　　　var li = document.createElement("li");

　　　　//添加 img
　　　　var img = document.createElement("img");

　　　　//设置 img 属性，如 id
　　　　img.setAttribute("id", "newImg");

　　　　//设置 img 图片地址
　　　　img.src = 'http:'+msg[0]['sample_url'];

　　　　li.appendChild(img);
　　　　ul.appendChild(li);
                    }
}
);
}
</script>
<ul id='i'></ul>
```
