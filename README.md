# html5
测试环境

* 操作系统：win7
* 服务器：Apache 2.2
* 浏览器版本：IE11, FF34, Chrome43

#Audio 例子
* 控制音频(单个或者多个)的播放，暂停，音量增大/减小，静音/非静音，
* 通过 onloadedmetadata 事件得到 音频的基本信息


#Video 例子
* 通过metedataLoadEvent事件得到 视频的基本信息
* 给视频添加字幕和隐藏字幕([各个浏览器的支持情况](https://developer.mozilla.org/en-US/Apps/Build/Audio_and_video_delivery/Adding_captions_and_subtitles_to_HTML5_video))
    * IE浏览器默认不识别 .vtt文件类型， 需要在 apache/conf/mime.tpyes 里面添加  **text/vtt						vtt**
    * FireFox track 标签要加 default才能显示字幕
* 对通过Canvas 正在播放的视频截屏([图片跨域问题](https://developer.mozilla.org/en-US/docs/Web/HTML/CORS_enabled_image))
    * 对于跨域视频，Chrome和FireFox只需要在video标签上面添加crossorigin="*" ，就可以截屏， IE下面有问题

#参考资料
* [http://www.html5tutorial.info](http://www.html5tutorial.info)
* [http://www.w3schools.com](http://www.w3schools.com)
* [添加字幕](https://developer.mozilla.org/en-US/Apps/Build/Audio_and_video_delivery/Adding_captions_and_subtitles_to_HTML5_video)