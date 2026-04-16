sdance2-fast-15s为15秒的满血fast模型
使用满血版即梦2 fast模型，请前往[https://api.xgapi.top/](https://api.xgapi.top/)
> 官方3.5折！官方3.5折！官方3.5折！官方3.5折！  15s视频仅需3.8元！！！！
> > 官方3.5折！官方3.5折！官方3.5折！官方3.5折！  15s视频仅需3.8元！！！！
> > > 官方3.5折！官方3.5折！官方3.5折！官方3.5折！  15s视频仅需3.8元！！！！

<br>
已支持满血版doubao-seedance-2-0-260128和doubao-seedance-2-0-fast-260128。
支持全能参考，视频编辑，视频延长等官方全功能。无需排队。
- 查看详情：[https://api.xgapi.top/pricing?model=doubao-seedance-2-0](https://api.xgapi.top/pricing?model=doubao-seedance-2-0)。<br>
- 对接文档：[https://xgapi.apifox.cn/444231142e0](https://xgapi.apifox.cn/444231142e0)<br>

生成示例：

### 参数说明
- 只有prompt为文生视频
- image 单图用
- images 多资源
  - 两张图默认首尾帧

### prompt使用说明
素材引用采用@占位符标记：

| 标题 |  |
| --- | --- |
| @1 / @图1 / @image1 |引用第一个素材
@2 / @图2 / @image2 | 引用第二个素材  |

全能参考限制：
| 类型 | 说明 |
| :--- | :--- |
| 图片 | 最多 9 张，可以传角色、场景、服装、商品、分镜图等 |
| 视频 | 最多 3 个，加起来不超过 15 秒，用来参考运镜、动作、转场 |
| 音频 | 支持 MP3，最多 3 个，总时长不超过 15 秒，可当背景音乐、音效或旁白参考 |
| 文字 | 用自然语言写你想要什么画面、什么动作就行，中英文都行 |
| 文件总数 | 图片 + 视频 + 音频全部加起来，最多 12 个 |
| 成片时长 | 4～15 秒自己选，生成出来的视频会自带音效和配乐 |


以此类推。
举例：

```
curl --location --request POST 'http://api.xgapi.top/v1/videos' \
--header 'Authorization: Bearer sk-666' \
--header 'Content-Type: application/json' \
--data-raw '{
  "model": "sdance2-fast-15s",
  "prompt": "@1带个帽子去@2的场景",
  "images": ["https://p16-dreamina-sign-sg.ibyteimg.com/tos-alisg-i-wopfjsm1ax-sg/a4963f3c438e40feb085fdeda992beea~tplv-wopfjsm1ax-aigc_resize:0:0.jpeg?lk3s=43402efa&x-expires=1775520000&x-signature=X6b5ZFCQXHOt3qhAFytodS7eyZs%3D&format=.jpeg", "https://v16-cc.capcut.com/64e56d72f078565e6e27a0873f8a4282/69d70e33/video/tos/alisg/tos-alisg-ve-14178-sg/oMPAEDeIpAm0TF8o1RCdTObgQPgeLisqGje6pb/?a=513641&bti=PDk6QC0yM2A%3D&&bt=6738&ft=GAAO2Inz7Thn6hOPXq8Zmo&mime_type=video_mp4&rc=aWQ8ZDdlNzw0Ozw7Zjc5O0BpajQ1bnI5cjt3OjYzODU6NEBfYzIvYmI1NS4xYDAvMDItYSM0NHNyMmRrNDNhLS1kMzFzcw%3D%3D&vvpl=1&l=20260402102550CCE1CA0C8AA5C716CAA3&btag=e000b0000"],
  "width": 1280, 
  "height": 720
}'
```

:::tip[]
"width": 1280,  "height": 720也可改为 "size": "1280*720"
:::

失败原因说明(来自官方，失败不扣费)：
RejectFace：参考材料中有真实人脸图片
OutputVideoRisk：视频结果不过审
OutputAudioRisk：输出的音频不过审
InputTextRisk：输入的提示词有敏感词
InputImageCopyright：输入的图像无版权

详细文档：[https://app.apifox.com/project/7826784](https://app.apifox.com/project/7826784)

联系方式：
<img width="184" height="188" alt="image" src="https://github.com/user-attachments/assets/78502534-886f-418c-9eaf-c01194b41d64" />
<img width="184" height="188" alt="image" src="https://github.com/user-attachments/assets/05bd7e32-2587-43ea-981a-b1aff8031442" />
