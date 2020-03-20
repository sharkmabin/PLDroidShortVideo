# PLDroidShortVideo

PLDroidShortVideo 是七牛推出的一款适用于 Android 平台的短视频 SDK，提供了包括美颜、滤镜、水印、断点录制、分段回删、视频编辑、混音特效、本地/云端存储在内的多种功能，支持高度定制以及二次开发。我们提供 80+ 功能供开发使用，申请 **0 元体验**可联系销售或[填写表单](https://jinshuju.net/f/IeOD89?ref=www.qiniu.com)获得产品试用权限。

## 1. 多版本功能分布
短视频SDK主要区分精简版、基础版、进阶版、专业版 4 个版本，不同版本的功能区别见如下表格

| 功能                         | 子功能                     |        精简版        |         基础版          |         进阶版          |          专业版          |
| :-------------------------- | :------------------------ | :------------------:| :---------------------: | :---------------------: | :----------------------: |
| **用户交互界面**              | **提供了一套完整的UI交互源码，可复用或自定义**         |          ✓           |            ✓            |            ✓            |            ✓             |
| **拍摄设置**                 | **摄像头采集**                                    |          ✓           |            ✓            |            ✓            |            ✓             |
|                             | **麦克风采集**                                    |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **视频采集参数定义**<br />*支持最高 1080P 拍摄，支持自定义视频采集源、采集画面的分辨率、采集画面的长宽比等参数* |          ✓          |          ✓          |          ✓          |          ✓           |
|                             | **音频采集参数定义**<br />*支持自定义音频采集源、音频格式、音频声道、音频采样率等参数* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **视频编码参数定义**<br />*支持自定义编码视频的码率、帧率、分辨率、H.264 编码方式等参数* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **音频编码参数定义**<br />*支持自定义编码音频的码率、采样率、声道数、AAC 编码方式等参数* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **拍摄时长设置**<br />*支持设置实际拍摄过程中的最大、最小拍摄时长* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **前后台切换**<br />*根据监听到 Application 的前后台状态自动停止和开始录制视频，默认从后台进入前台自动开始录制* |          ✓          |          ✓          |          ✓          |         ✓         |
|                             | **摄像头切换**<br />*支持切换前后摄像头进行拍摄*             |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **闪光灯设置**<br />*支持开关闪光灯用于拍摄时的补光*          |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **画面镜像**<br />*支持设置是否镜像预览画面和编码画面*       |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **画面对焦**<br />*支持手动对焦和自动对焦*                  |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **焦距调节**<br />*支持手动调节画面焦距进行放大、缩小*       |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **曝光调节**<br />*支持调整曝光度参数*                     |          ✓          |            ✓            |            ✓            |            ✓             |
| **拍摄模式**                 | **横屏拍摄**<br />*支持根据设备的方向自动确定竖屏、横屏拍摄*  |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **分段拍摄**<br />*支持拍摄过程中实现连续多次拍摄、断点续拍、回删* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **静音拍摄**<br />*支持静音拍摄*                          |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **音频录制**<br />*支持纯音频录制*                        |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **屏幕录制**<br />*支持对整个屏幕区域进行录制，实现整体的录制效果* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **变速拍摄**<br />*支持设置拍摄时的快/慢速率，目前支持 5 种拍摄速率（默认正常速率，只支持 2 的倍数，或 1/2 的倍数）* |        ✗        |        ✓        |        ✓        |        ✓         |
|                             | **分屏拍摄（合拍）**<br />*可以根据素材视频（或图片）进行合拍，生成双画面视频* |            ✗            |            ✗            |          ✓          |            ✓             |
| **实时处理**                 | **实时截图**<br />*支持拍摄时实时截图拍照保存到本地*         |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **实时预览**<br />*支持实时本地预览*                      |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **实时美颜**<br />*支持拍摄时启用美颜功能，支持设置美颜、美白、红润 3 种效果并调节强度* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **实时滤镜**<br />支持*拍摄时启用滤镜功能，支持自由调节多种滤镜效果（33种）* |            ✗           | ✓<br />提供 10 种滤镜效果 | ✓<br />提供 33 种滤镜效果 | ✓<br />提供 33 种滤镜效果  |
|                             | **实时水印**<br />*支持拍摄时添加静态水印，支持设置水印位置、大小、透明度，设置作用时间范围* |            ✗            |          ✓          |            ✓            |            ✓             |
|                             | **背景音乐**<br />*支持拍摄前选择本地文件作为背景音乐*       |            ✗            |          ✓          |            ✓            |            ✓             |
| **基础编辑**                 | **视频导入**<br />*支持本地视频快速导入后编辑*               |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **编辑预览**<br />*支持编辑时实时预览本地效果*               |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **时长剪裁**<br />*支持时长裁剪，按照给定的时间范围生成一个 mp4 文件* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **本地转码**<br />*支持按照给定的码率、帧率等参数，生成一个 mp4 文件* |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **视频旋转**<br />*支持按照给定的目标旋转角度，生成一个 mp4 文件*       |            ✗            |          ✓          |            ✓            |            ✓             |
|                             | **画面剪裁**<br />*支持画面裁剪，按照视频画面大小（原比例、指定区域）精确裁剪视频生成一个mp4文件* |            ✗            |            ✗            |          ✓          |          ✓         |
| **特效编辑**                 | **视频旋转特效**<br />*支持设置视频左右上下旋转，实时预览旋转效果*               |          ✗          |            ✓            |            ✓            |            ✓             |
|                             | **单音频混音**<br />*支持给视频文件添加单音频，实现混音效果*       |            ✗            |          ✓          |            ✓            |            ✓             |
|                             | **滤镜特效**<br />*支持给视频文件添加滤镜效果，默认支持 33 种滤镜效果* |            ✗           | ✓<br />提供 10 种滤镜效果 | ✓<br />提供 33 种滤镜效果 | ✓<br />提供 33 种滤镜效果  |
|                             | **涂鸦特效**<br />*支持画笔尺寸和颜色调整，支持设置特效显示的时间范围* |            ✗            |          ✓          |            ✓            |            ✓             |
|                             | **字幕特效**<br />*支持给视频文件添加文字特效，支持设置文字内容，字体大小，字体颜色，透明度，旋转，位置等，支持设置特效显示的时间范围* |        ✗        |        ✓       |        ✓        |        ✓         |
|                             | **水印特效**<br />*支持给视频文件添加静态、动态水印，并且能够自由设置水印的大小、位置、透明度、旋转角度，支持设置特效显示的时间范围，可以自定义素材或使用供应商提供的收费素材* |        ✗        |          ✓          |            ✓            |            ✓             |
|                             | **贴纸特效**<br />*支持给视频文件添加静态贴纸，并且能够自由设置贴纸大小、位置、旋转角度，支持设置特效显示的时间范围，可以自定义素材或使用供应商提供的收费素材* |        ✗        |        ✓        |            ✓            |            ✓            |
|                             | **时间特效**<br />*支持对视频文件进行整体变速、分段变速，支持5种变速效果（极慢、慢、正常、快、极快）* |            ✗            |          ✓          |         ✓        |       ✓       |
|                             | **时光倒流**<br />*支持 1 种倒放操作（即时光倒流特效）* |            ✗            |          ✗          |         ✓        |       ✓       |
|                             | **音乐唱片**<br />*支持音频录制的过程中，增加图片旋转效果，输出为 mp4 文件* |          ✗          |          ✗          |            ✓            |            ✓             |
|                             | **多音频混音**<br />*支持给视频文件添加多个背景音乐，支持调整视频原声、背景音乐音量，支持设置多个背景音乐有效时间区域，支持自己录音或者选用本地音乐* |        ✗        |      ✗      |      ✗       |      ✓     |
|                             | **MV 特效**<br />*支持给视频文件添加 MV 效果，默认提供 4 种 MV 特效，MV 特效素材需要客户自行按要求制作* |         ✗          |          ✗          |            ✗            |            ✓             |
| **多素材编排**                | **视频拼接**<br />*支持设置多个视频按照前后顺序导入拼接生成一个 mp4 文件* |            ✗            |          ✗          |         ✓         |       ✓       |
|                             | **GIF 动画**<br />*支持基于多个图片或视频直接导出 GIF 动图*     |          ✗           |          ✗          |            ✓            |            ✓             |
|                             | **图片拼接**<br />*支持设置多个图片按照前后顺序导入拼接生成一个 mp4 文件* |            ✗           |          ✗          |            ✓            |            ✓             |
|                             | **基础转场**<br />*支持在视频图片片段之间，增加淡入淡出效果*   |           ✗            |          ✗          |            ✓            |            ✓             |
|                             | **过场字幕**<br />*支持在视频之间增加转场字幕，支持定义转场字幕的背景色、持续时间、支持文字和图片特效，支持旋转、放大、位置移动、淡入淡出 4 种效果* |            ✗            |            ✗            |            ✓             |          ✓          |
|                             | **视频合成**<br />*支持设置多个视频合并为一个视频，支持设置每一个视频的位置、大小、开始播放时间等* |          ✗           |            ✗            |          ✗          |          ✓           |
|                             | **图片 & GIF 图 & 视频混拼**<br />*支持设置多个视频和图片按照前后顺序导入拼接生成一个 mp4 文件* |          ✗           |            ✗            |          ✗          |           ✓          |
| **其他功能**                 | **草稿箱**<br />*支持将当前录制的片段与设置项存入草稿箱*     |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **接口扩展**<br />*扩展接口支持对接第三方美颜特效等增值能力*                 |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **外部裸数据导入**<br />*支持外部音视频裸数据导入，生成 mp4 文件*    |          ✗          |          ✗          |            ✗            |            ✓             |
|                             | **View 录制**<br />*支持 View 录制*    |          ✗          |          ✗          |            ✗            |            ✓             |
| **视频播放**                 | **播放器 SDK**                                                |          ✓          |            ✓            |            ✓            |            ✓             |
| **上传分发**                 | **视频上传**                                                 |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **断点续传**                                                 |          ✓          |            ✓            |            ✓            |            ✓             |
|                             | **上传加速**                                                 |          ✓          |            ✓            |            ✓            |            ✓             |

增值能力方面，需要单独选购，在视频拍摄或视频编辑阶段增加，4个版本都支持相关开放接口。

| **功能**                                                                            |
| ---------------------------------------------------------------------------------- |
| **高级美颜**<br />*拍摄设置大眼、瘦脸、V脸、下巴调整、短脸、小鼻效果，并支持调节强度*           |
| **人脸贴纸**<br />*支持人脸识别，进行人脸 2D、3D 贴纸操作*                                 |
| **手势识别**<br />*可以对拍摄的人物的特定手势进行识别，配合其他特效*                         |
| **AR 特效**<br />*支持拍摄时设置 AR 特效*                                               |
| **变声混响**<br />*拍摄时对录制的人音进行变声（如萝莉、大叔）和混响效果等操作（如 KTV、会堂）*    |
| **类抖音特效**<br />*滤镜效果，支持抖动、幻觉、灵魂出窍等数种抖音特效*                        |
| **背景抠图**<br />*将画面中的绿色元素(比如纯绿背景)抠除，替换成其他的元素，比如动态背景/ PPT 等* |

## 2. 设备以及系统要求

- 设备要求：搭载 Android 系统的设备
- 系统要求：Android 4.3(API 18) 及其以上

## 3. 使用方法

请参考开发者中心文档：[PLDroidShortVideo 文档](https://developer.qiniu.com/pili/sdk/3734/short-video-android-sdk)

**注意：若无法 clone 本 repo，可点击[下载](https://sdk-release.qnsdk.com/PLDroidShortVideo-v3.1.1.zip)**

## 4. 声明

本短视频 SDK 需授权方可使用，可通过 400-808-9176 转 2 号线联系七牛商务咨询，或者 [通过工单](https://support.qiniu.com/?ref=developer.qiniu.com) 联系七牛的技术支持。

## 5. 反馈及意见

当你遇到任何问题时，可以通过在 GitHub 的 repo 提交 issues 来反馈问题，请尽可能的描述清楚遇到的问题，如果有错误信息也一同附带，并且在 Labels 中指明类型为 bug 或者其他。

[通过这里查看已有的 issues 和提交 Bug](https://github.com/pili-engineering/PLDroidShortVideo/issues)
~