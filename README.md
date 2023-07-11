# douyin-wss
抖音网页版私信聊天WSS抓包分析

> 建议移步 [https://github.com/YunzhiYike/douyin-live](https://github.com/YunzhiYike/douyin-live) 该项目更新更及时全面。本项目经年未更，无法保障可用性。

## 接收到文本消息
```json
{
  "type": 0,
  "isShareText": false,
  "item_type_local": -1,
  "richTextInfos": [],
  "text": "消息内容",
  "createdAt": 0,
  "is_card": false,
  "msgHint": "",
  "aweType": 700
}
```

## 接收到抖音内置表情

```json
{
  "type": 0,
  "isShareText": false,
  "item_type_local": -1,
  "richTextInfos": [],
  "text": "[微笑]",
  "createdAt": 0,
  "is_card": false,
  "msgHint": "",
  "aweType": 700
}
```

## 接受到gif表情

```json
{
  "aweType": 500,
  "createdAt": 0,
  "display_name": "",
  "height": 240,
  "image_id": 6752145780640842000,
  "image_type": "gif",
  "is_card": false,
  "msgHint": "",
  "package_id": 0,
  "resource_type": 0,
  "show_notice": false,
  "updateConversationTime": true,
  "url": {
    "data_size": 0,
    "height": 0,
    "uri": "joker/weshine/d53f03fc76f9b0c82fd1bf5407b89bda.gif",
    "url_list": [
      "https://p26-sign.douyinpic.com/obj/joker/weshine/d53f03fc76f9b0c82fd1bf5407b89bda.gif?x-expires=1684044000&x-signature=hxaEiMTJx5280LaDrEBiwlgsXPk%3D&from=2526598866",
      "https://p9-sign.douyinpic.com/obj/joker/weshine/d53f03fc76f9b0c82fd1bf5407b89bda.gif?x-expires=1684044000&x-signature=2LKlh%2Bi5WauKcH3x90lMkgDunrY%3D&from=2526598866",
      "https://p26-sign.douyinpic.com/obj/joker/weshine/d53f03fc76f9b0c82fd1bf5407b89bda.gif?x-expires=1684044000&x-signature=hxaEiMTJx5280LaDrEBiwlgsXPk%3D&from=2526598866"
    ],
    "width": 0
  }
}
```


## 接收到语音

```json
{
  "height": 0,
  "data_size": 0,
  "uri": "douyin-user-audio-file/7097479842803187751.mpeg",
  "url_list": [
    "https://sf3-sign.douyinstatic.com/douyin-user-audio-file/7097479842803187751.mpeg?x-expires=1684046800&x-signature=dcAnFEvKNJDNtbjIbyjbNim0Eo4%3D",
    "https://sf26-sign.douyinstatic.com/douyin-user-audio-file/7097479842803187751.mpeg?x-expires=1684046800&x-signature=%2FaHfNrXX0Rl5uw02u6qnMKHk%2BXs%3D"
  ],
  "width": 0
}
```

## 接收到用户图片

```json
{
  "aweType": 2702,
  "check_pics": [],
  "cover_height": 726,
  "cover_width": 1046,
  "createdAt": 1652511029140,
  "encodeTime": 11,
  "from_gallery": 1,
  "is_card": false,
  "mass_msg": 1,
  "md5": "25bd2187f8f7cb0481c02e35d1bd5095",
  "msgHint": "",
  "prev_id": 7097480824299260000,
  "resource_url": {
    "data_size": 101531,
    "height": 0,
    "large_url_list": [
      "https://p26-sign.douyinpic.com/tos-cn-o-00061/7e659c55a5fb4324928e97900c28b7f1~tplv-x-get:large.image?x-expires=1684047600&x-signature=jQ9GfzbRWRUtIInL6r4NJDsBYvg%3D&from=2526598866"
    ],
    "md5": "25bd2187f8f7cb0481c02e35d1bd5095",
    "medium_url_list": [
      "https://p3-sign.douyinpic.com/tos-cn-o-00061/7e659c55a5fb4324928e97900c28b7f1~tplv-x-get:medium.image?x-expires=1684047600&x-signature=tGszyhw1FYI8APM7vBZF2Gjb1%2FM%3D&from=2526598866"
    ],
    "oid": "tos-cn-o-00061/7e659c55a5fb4324928e97900c28b7f1",
    "origin_url_list": [
      "https://p3-sign.douyinpic.com/tos-cn-o-00061/7e659c55a5fb4324928e97900c28b7f1~tplv-x-get:.image?x-expires=1684047600&x-signature=K9Y47b2DmQaqON9ld%2BM%2Foy78uXU%3D&from=2526598866"
    ],
    "skey": "84120f5012242af2abd66f52b059a16059d2bb2bc9807a04e302c1f918113df2",
    "thumb_url_list": [
      "https://p26-sign.douyinpic.com/tos-cn-o-00061/7e659c55a5fb4324928e97900c28b7f1~tplv-x-get:thumb.image?x-expires=1684047600&x-signature=AEW7dXvYdgarNgJzgtPdjAIk2QE%3D&from=2526598866"
    ],
    "width": 0
  },
  "root_id": 7097480824299260000,
  "sendRaw": false
}
```
> 图片需解密，解密方法未知

## 收到位置消息
```json
{
  "aweType": 0,
  "aweme_poi_id": "6601265443279734788",
  "cover_info": {
    "resource_url": {
      "data_size": 0,
      "height": 0,
      "uri": "douyin-user-image-file/d3eb88f67cf6b10ed454ec79e48648cf",
      "url_list": [
        "https://p9-sign.douyinpic.com/obj/douyin-user-image-file/d3eb88f67cf6b10ed454ec79e48648cf?x-expires=1684047600&x-signature=XG1pVfOVlBMkodo29bK0VCigltQ%3D&from=2526598866",
        "https://p3-sign.douyinpic.com/obj/douyin-user-image-file/d3eb88f67cf6b10ed454ec79e48648cf?x-expires=1684047600&x-signature=nV%2FYpvjA%2FK8CiaXfDJdjey8KWLU%3D&from=2526598866",
        "https://p6-sign.douyinpic.com/obj/douyin-user-image-file/d3eb88f67cf6b10ed454ec79e48648cf?x-expires=1684047600&x-signature=x4l%2FxLWqS8XhL%2Bv7qjT7hA3M%2BFU%3D&from=2526598866"
      ],
      "width": 0
    }
  },
  "createdAt": 0,
  "is_card": false,
  "latitude": 24.617908631273124,
  "longitude": 118.04502062375067,
  "msgHint": "",
  "poi_address": "福建省厦门市集美区诚毅北大街",
  "poi_id": "",
  "poi_name": "金海豚广场"
}
```

## 接收到抖音视频消息

```json
{
  "aweType": 800,
  "awemeType": 0,
  "content_name": "nickname",
  "content_thumb": {
    "data_size": 0,
    "height": 720,
    "uri": "100x100/aweme-avatar/tos-cn-i-0813_b5af190295434238bf6151da514a1c1c",
    "url_list": [
      "https://p26-sign.douyinpic.com/obj/aweme-avatar/tos-cn-i-0813_b5af190295434238bf6151da514a1c1c?x-expires=1684047600&x-signature=l1YIWVBv58IH6%2BRbNiXLY5xOlKQ%3D&from=2526598866",
      "https://p3-sign.douyinpic.com/obj/aweme-avatar/tos-cn-i-0813_b5af190295434238bf6151da514a1c1c?x-expires=1684047600&x-signature=nxPR5y8GrvLgz7f3U9eAsDSOS88%3D&from=2526598866",
      "https://p6-sign.douyinpic.com/obj/aweme-avatar/tos-cn-i-0813_b5af190295434238bf6151da514a1c1c?x-expires=1684047600&x-signature=Ih37%2FLLqQrq1ycl%2Be2LBeHxoLI8%3D&from=2526598866"
    ],
    "width": 720
  },
  "content_title": "",
  "cover_height": 1280,
  "cover_url": {
    "data_size": 0,
    "height": 720,
    "uri": "tos-cn-p-0015/d9bb9134d35b45b8b593b705958e7780",
    "url_list": [
      "https://p3-sign.douyinpic.com/obj/tos-cn-p-0015/d9bb9134d35b45b8b593b705958e7780?x-expires=1684047600&x-signature=v%2B%2BHwWL3hcoV0wPPdLbEEih7Cng%3D&from=2526598866",
      "https://p9-sign.douyinpic.com/obj/tos-cn-p-0015/d9bb9134d35b45b8b593b705958e7780?x-expires=1684047600&x-signature=hkK%2FRCIOb8juRxsk1BGtH96A%2F5E%3D&from=2526598866",
      "https://p26-sign.douyinpic.com/obj/tos-cn-p-0015/d9bb9134d35b45b8b593b705958e7780?x-expires=1684047600&x-signature=5hSb%2FvgjuPZD9hq2npTgob0pDKE%3D&from=2526598866"
    ],
    "width": 720
  },
  "cover_width": 720,
  "createdAt": 0,
  "hot_spot_create_time": 1652514463,
  "is_card": false,
  "is_hot_spot_video": false,
  "itemId": "7097473243912621351",  // 
  "msgHint": "",
  "need_skip_strange": 0,
  "secUID": "MS4wLjABAAAAhJYrMAP2pH4n4ZTi50fFBl_cFbgEueu0bEqVK_F5-R1MF3CitsWUtzn_bP9pUv2S",
  "uid": "1200310293640376"
}
```

itemId拼接https://www.douyin.com/video/后形成抖音视频URL
