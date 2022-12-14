
# [<img src="https://www.hankmi.com/favicon.ico" width="60" height="60" align="center" />](https://www.hankmi.com) HankMi官方网站

## 抬腕视频开放平台

抬腕视频遵循友善、绿色的开放原则，为安卓智能手表生态贡献力量。我们提供可能是最简单的接入方式，Hankode不可阻挡，无需人工审核和确认，接入即用。  
1.要接入Hankode，你需要为应用申请存储空间权限，在 `AndroidManifest.xml` 中加入以下权限声明：  
~~~
android.permission.WRITE_EXTERNAL
~~~
申请权限时我们希望你能为用户提供相关权限申请说明。  
  
2.在需要播放视频时生成Hankode并写入到指定路径，首先生成以下格式的Hankode到一个自定的文本型变量：  
~~~
hmmedia=[欲播放的视频绝对路径/网络视频直播地址]
~~~
  
3.生成完成后，将此变量的内容以utf-8编码保存到以下路径中：  
~~~
[设备存储卡路径] + /HankMi/cache/media/keydata.hmd
~~~
  
4.生成完成后，直接跳转抬腕视频 `com.hankmi.media` 即可。为了用户操作更加直观，我们建议在跳转应用前应用给出`H码握手成功，请在抬腕视频继续操作`的提示。  
  
5.未防止跳转后用户不操作导致Hankode导出成缓存垃圾文件，可在你的应用`窗口被恢复`等事件中，删除写出的`keydata.hmd`文件，但这不是必须的，因为此文件后续仍可被覆盖。  
  
  
抬腕视频目前支持的本地视频播放格式：mp4、mov、avi、3gp、flv
