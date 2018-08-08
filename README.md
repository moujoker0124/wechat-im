# wechat-im
### 微信小程序即时通讯

开发这个项目付出了我很多心血，如果对你有帮助和启发的话，希望在`GitHub`上给个`star`！也是对我工作的支持和肯定！

## 介绍：
wechat-im是一个可以让你在小程序平台快速实现即时通讯功能的完整项目。

## 特性：
- [x] 目前项目中已使用webSocket，实现了IM的通信功能！目前包括会话列表页面、会话页面及好友页面。支持使用nodejs开启本地WebSocket服务。
- [x] 支持发送文本、图片、语音，支持输入法的emoji表情
- [x] 支持拍照，图库选择图片、图片预览
- [x] 支持切换到文本输入时，显示发送按钮。
- [x] 支持语音播放及播放动画。
- [x] 支持配置录制语音的最短及最长时间。
- [x] 支持配置自定义事件。
- [x] 支持聊天消息按时间排序。
- [x] 支持发送消息后，页面回弹到最底部。
- [x] 使用了最新的语音播放接口，同时兼容了低版本的语音播放接口。
- [x] 消息发送中、发送成功、发送失败的状态更新
- [x] 支持消息发送失败情况下，点击重发按钮重新发送
- [x] 优化时间气泡显示逻辑，相邻信息大于5分钟显示后者信息的时间
- [x] 在页面最上方增加了会话状态的UI展示
- [x] 自定义功能，显示自定义气泡。
- [x] 通过解析语音或图片消息信息，优先读取本地文件。
- [x] 实现了文件存储算法，保证10M存储空间内的语音和图片文件均为最新。
- [x] 最低支持微信基础库版本为1.4.0
- [x] 各消息类型和各功能均已模块化，让你在浏览代码时愉悦轻松。（其实这算不上组件特性。。。）

## 目前不支持的功能：
- 如果要使用群聊，目前的UI中，头像旁并没有展示成员昵称。
- 本地没有存储历史聊天消息。这个原因请看文章结尾。
- 目前WebSocket所有功能仅供学习和参考，若想商用，请自行开发。

## 如何安装使用

#### 1. 开发者工具导入项目

#### 2. 搭建本地WebSocket服务
```
安装依赖 npm install nodejs-websocket
运行 项目.server文件夹下的web-socket-server.js文件即可开启服务
```
#### 3. 使用开发者工具运行项目

### 整体效果图（加载有些慢）
我们先来看下效果 (因录制软件问题，图中的一些按钮的变色了，线条也少了很多像素。。。)

- 发送图片和图片预览

<img src="https://github.com/unmagic/.gif/blob/master/wechat-im/发送图片和图片预览.gif" width="30%" alt="发送图片和图片预览"/>

- 消息重发和发送自定义消息

<img src="https://github.com/unmagic/.gif/blob/master/wechat-im/消息重发和发送自定义消息.gif" width="30%" alt="消息重发和发送自定义消息"/>

- 发送语音消息

<img src="https://github.com/unmagic/.gif/blob/master/wechat-im/语音.gif" width="30%" alt="发送语音消息"/>

使用中有什么问题的话，可以在博客或GitHub上联系我。我会及时回复。

谢谢大家！

### LINK

[Document](https://blog.csdn.net/sinat_27612147/article/details/78456363)

[LICENSE](https://github.com/unmagic/wechat-im/blob/master/LICENSE)
