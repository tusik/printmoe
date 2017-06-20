---
name: 直接输出模式
---

# 直接输出模式

使用我的服务器作为cdn缓存直接输出壁纸

集成json模式下的所有参数（除了limit，因为只会输出一张壁纸）

## 范例 

```
http://api.print.moe/api.jpg

http://api.print.moe/api.jpg?order=3 
```

![壁纸](http://api.print.moe/api.jpg)

![壁纸](http://api.print.moe/api.jpg?order=3)

## 没有符合条件的图片

![404](http://api.print.moe/api.jpg?order=3&tag=efsefsedfeefeefdesfef)
