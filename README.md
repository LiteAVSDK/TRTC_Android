# 腾讯云实时音视频 TRTC SDK

_[English](README.en.md) | 简体中文_
## 产品介绍

腾讯实时音视频（Tencent Real-Time Communication，TRTC），将腾讯多年来在网络与音视频技术上的深度积累，以多人音视频通话和低延时互动直播两大场景化方案，通过腾讯云服务向开发者开放，致力于帮助开发者快速搭建低成本、低延时、高品质的音视频互动解决方案，[更多](https://cloud.tencent.com/document/product/647/16788)...

> TRTC SDK 支持Web、Android、iOS、Windows以及Flutter、小程序等所有主流平台， [更多平台](https://github.com/LiteAVSDK?q=TRTC_&type=all&sort=)...



## 更新日志

### Version 9.7 @ 2022.04.06

**功能优化：** 
- iOS & Android：优化 Music 音质的效果；
  > Tips：全平台均可通过 API ： [TRTCCloud.startLocalAudio (TRTCAudioQualityMusic)](https://liteav.sdk.qcloud.com/doc/api/zh-cn/group__TRTCCloud__android.html#a1dadf09b10a2d128e4cef11707934329) 开启Music 音质，下同）
- Windows：优化 Music 音质下的采播效果，降低对音质的损伤；
- Windows：提升部分专业声卡上的兼容性适配问题，有效提升音质；
- Windows：第三方进程混音优化，让第三方进程混音功能可以适配更多的场景；

**缺陷修复：**
- 全平台：修复 CDN 播放偶现视频画面花屏的问题；
- iOS & Android：修复直播播放听筒扬声器切换无效的问题；
- iOS & Android：修复通过 API 设置 Music 音质时实际音质不符合预期的问题；
- iOS：修复软编码过程中偶现的内存泄露问题；
- iOS：修复本地视频画面渲染，偶现无首帧回调的问题；
- Windows：修复屏幕分享模式下鼠标采集偶现的异常崩溃；
- Windows：修复 Music 音质下，扬声器播放声音异常问题；
- Windows：修复部分摄像头 startCameraDeviceTest 无法正常打开的问题；

更早期的版本更新历史请点击  [更多](https://cloud.tencent.com/document/product/647/46907)...


## 目录说明

```bash
├─ TRTC-API-Example // TRTC API Example，包括视频通话、语音通话的基础功能以及一些高级功能
|  ├─ Basic                 // 演示 TRTC 基础功能示例代码
|  |  ├─ AudioCall                 // 演示 TRTC 音频通话的示例代码
|  |  ├─ VideoCall                 // 演示 TRTC 视频通话的示例代码
|  |  ├─ Live                      // 演示 TRTC 视频互动直播的示例代码
|  |  ├─ VoiceChatRoom             // 演示 TRTC 语音互动直播的示例代码
|  |  ├─ ScreenShare               // 演示 TRTC 录屏直播的示例代码
|  ├─ Advanced              // 演示 TRTC 高级功能示例代码
|  |  ├─ StringRoomId              // 演示 TRTC 字符串房间号示例代码
|  |  ├─ SetVideoQuality           // 演示 TRTC 画质设定示例代码
|  |  ├─ SetAudioQuality           // 演示 TRTC 音质设定示例代码
|  |  ├─ SetRenderParams           // 演示 TRTC 渲染控制示例代码
|  |  ├─ SpeedTest                 // 演示 TRTC 网络测速示例代码
|  |  ├─ PushCDN                   // 演示 TRTC CDN发布示例代码
|  |  ├─ CustomCamera              // 演示 TRTC 自定义视频采集&渲染发布示例代码
|  |  ├─ SetAudioEffect            // 演示 TRTC 设置音效示例代码
|  |  ├─ SetBackgroundMusic        // 演示 TRTC 设置背景音乐示例代码
|  |  ├─ LocalVideoShare           // 演示 TRTC 本地视频文件分享示例代码
|  |  ├─ LocalRecord               // 演示 TRTC 本地视频录制示例代码
|  |  ├─ JoinMultipleRoom          // 演示 TRTC 加入多个房间示例代码
|  |  ├─ SEIMessage                // 演示 TRTC 收发SEI消息示例代码
|  |  ├─ SwitchRoom                // 演示 TRTC 快速切换房间示例代码
|  |  ├─ RoomPk                    // 演示 TRTC 跨房PK示例代码
|  |  ├─ ThirdBeauty               // 演示 TRTC 第三方美颜示例代码
|  
|  
├─ SDK 
│  ├─README.md     // 提供有TRTC SDK最新版本的下载地址
```



## 联系我们
- 如果你遇到了困难，可以先参阅 [常见问题](https://cloud.tencent.com/document/product/647/43018)；

- 如果你想了解TRTC SDK在复杂场景下的应用，可以参考[更多场景案例](https://cloud.tencent.com/document/product/647/57486)；

- 完整的 API 文档见 [SDK 的 API 文档](http://doc.qcloudtrtc.com/md_introduction_trtc_Android_%E6%A6%82%E8%A7%88.html)；
- 如果需要售后技术支持, 你可以点击[这里](https://cloud.tencent.com/document/product/647/19906)；
- 如果发现了示例代码的 bug，欢迎提交 issue；
