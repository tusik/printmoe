---
name: 如何使用
---

# 如何使用

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

### 详细参数解析

- order：{score|width|height|created_at}：以list存储，0为score
- desc：{asc|desc}：以list存储，0为asc，升序

### 范例

```
http://print.moe/api?limit=3&page=1&days=10&desc=1&order=0&w_max=3500&w_min=1200
```
### 返回范例

```
[{"source": "http://dekodere.deviantart.com/art/Kaiki-Deishuu-Wallpaper-414773883", "tags": "all_male bakemonogatari black_eyes black_hair dekodere kaiki_deishuu male monogatari_(series) short_hair snow umbrella vector", "has_children": "0", "author": "RyuZU", "creator_id": 156425, "rating": "", "is_held": null, "sample_url": "//konachan.com/sample/819e274c14c3104c42873a88050acf7f/Konachan.com%20-%20244812%20sample.jpg", "kid": "244812", "created_at": "1497385745", "is_shown_in_index": "1", "id": 64, "height": 1080, "file_url": "//konachan.com/image/819e274c14c3104c42873a88050acf7f/Konachan.com%20-%20244812%20all_male%20bakemonogatari%20black_eyes%20black_hair%20dekodere%20kaiki_deishuu%20male%20monogatari_%28series%29%20short_hair%20snow%20umbrella%20vector.png", "md5": "819e274c14c3104c42873a88050acf7f", "jpeg_url": "//konachan.com/jpeg/819e274c14c3104c42873a88050acf7f/Konachan.com%20-%20244812%20all_male%20bakemonogatari%20black_eyes%20black_hair%20dekodere%20kaiki_deishuu%20male%20monogatari_%28series%29%20short_hair%20snow%20umbrella%20vector.jpg", "file_size": "420413", "width": 1920, "preview_url": "//konachan.com/data/preview/81/9e/819e274c14c3104c42873a88050acf7f.jpg", "score": 0}, {"source": "http://drawingshit.deviantart.com/art/Yuno-340050652", "tags": "blush brown_hair close hidamari_sketch short_hair tagme_(artist) vector yuno", "has_children": "0", "author": "RyuZU", "creator_id": 156425, "rating": "", "is_held": null, "sample_url": "//konachan.com/sample/ff84991414ce2b506be850a5162c5dc1/Konachan.com%20-%20244975%20sample.jpg", "kid": "244975", "created_at": "1497663051", "is_shown_in_index": "1", "id": 79941, "height": 1600, "file_url": "//konachan.com/image/ff84991414ce2b506be850a5162c5dc1/Konachan.com%20-%20244975%20blush%20brown_hair%20close%20hidamari_sketch%20short_hair%20tagme_%28artist%29%20vector%20yuno.png", "md5": "ff84991414ce2b506be850a5162c5dc1", "jpeg_url": "//konachan.com/jpeg/ff84991414ce2b506be850a5162c5dc1/Konachan.com%20-%20244975%20blush%20brown_hair%20close%20hidamari_sketch%20short_hair%20tagme_%28artist%29%20vector%20yuno.jpg", "file_size": "1207577", "width": 2560, "preview_url": "//konachan.com/data/preview/ff/84/ff84991414ce2b506be850a5162c5dc1.jpg", "score": 0}, {"source": "http://drawingshit.deviantart.com/art/Koyomi-Araragi-331010813", "tags": "all_male araragi_koyomi bakemonogatari black_hair male monogatari_(series) short_hair tagme_(artist) vector", "has_children": "0", "author": "RyuZU", "creator_id": 156425, "rating": "", "is_held": null, "sample_url": "//konachan.com/sample/5e59b0e60ddc7bbb0c5988d4516ff29b/Konachan.com%20-%20244971%20sample.jpg", "kid": "244971", "created_at": "1497662563", "is_shown_in_index": "1", "id": 79945, "height": 1600, "file_url": "//konachan.com/image/5e59b0e60ddc7bbb0c5988d4516ff29b/Konachan.com%20-%20244971%20all_male%20araragi_koyomi%20bakemonogatari%20black_hair%20male%20monogatari_%28series%29%20short_hair%20tagme_%28artist%29%20vector.png", "md5": "5e59b0e60ddc7bbb0c5988d4516ff29b", "jpeg_url": "//konachan.com/jpeg/5e59b0e60ddc7bbb0c5988d4516ff29b/Konachan.com%20-%20244971%20all_male%20araragi_koyomi%20bakemonogatari%20black_hair%20male%20monogatari_%28series%29%20short_hair%20tagme_%28artist%29%20vector.jpg", "file_size": "1556096", "width": 2560, "preview_url": "//konachan.com/data/preview/5e/59/5e59b0e60ddc7bbb0c5988d4516ff29b.jpg", "score": 0}]
```
