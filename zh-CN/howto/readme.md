---
name: 如何使用
---

# 基本使用使用

  默认以score进行降序排序
  
## 基本参数


|参数名|类型|备注|默认|
|:--:|:--:|:--------------------------------:|:--:|
|limit|Int|最大100超过100还是100|1|
|page|Int|页面|1|
|author|String|作者||
|days|Int|多少天前的范围|1(当天)|
|w_max|Int|最大宽度||
|w_min|Int|最小宽度|
|h_max|Int|最大高度|
|h_min|Int|最小高度|
|order|String|排序方式|0|
|desc|Int|是否降序|0|
|tag|String|检索单词

### 详细参数解析

- order：{score|width|height|created_at}：以list存储，0为score
- desc：{asc|desc}：以list存储，0为asc，升序

### 范例

```
http://api.print.moe/api.json?limit=1&page=1&days=10&desc=1&order=0&w_max=3500&w_min=1200
```
### 返回范例

返回json数组

```json
[
    {
        "kid": "244305",
        "jpeg_url": "//konachan.com/image/45b654487d8884cd4afc23d1c5c8be21/Konachan.com%20-%20244305%20bikini%20blush%20breasts%20cleavage%20ilya_kuvshinov%20navel%20original%20pink_eyes%20short_hair%20swimsuit%20white.jpg",
        "is_held": null,
        "author": "mattiasc02",
        "id": 403,
        "width": 1920,
        "has_children": "0",
        "is_shown_in_index": "1",
        "source": "https://www.pixiv.net/member_illust.php?mode=medium&illust_id=63041341",
        "file_size": "170506",
        "file_url": "//konachan.com/image/45b654487d8884cd4afc23d1c5c8be21/Konachan.com%20-%20244305%20bikini%20blush%20breasts%20cleavage%20ilya_kuvshinov%20navel%20original%20pink_eyes%20short_hair%20swimsuit%20white.jpg",
        "created_at": "1496949602",
        "creator_id": 140316,
        "sample_url": "//konachan.com/sample/45b654487d8884cd4afc23d1c5c8be21/Konachan.com%20-%20244305%20sample.jpg",
        "score": 117,
        "preview_url": "//konachan.com/data/preview/45/b6/45b654487d8884cd4afc23d1c5c8be21.jpg",
        "rating": "",
        "md5": "45b654487d8884cd4afc23d1c5c8be21",
        "tags": "bikini blush breasts cleavage ilya_kuvshinov navel original pink_eyes short_hair swimsuit white",
        "height": 1080
    }
]
```
