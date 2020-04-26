**双生视界:女仆咖啡枪**
**雙生視界：少女咖啡槍**
**Girl Cafe cancer**
**ガールカフェガン**

配置模型推荐用Live2DViewerEX，比较容易配置。

**Live2d模型提取和语音提取方法

Live2d模型提取参考：[链接](https://www.perfare.net/1564.html)。
模型已经提取出来了。

语音提取方法：[参考](https://eiknya.github.io)
音频文件在手机存储 \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android (日服)
国服的把jp.Marvelous.girlcafegun换成有bilibili的
人物语音在手机存储  \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\English(US)
文件Vo_Normal开头的是人物语音。

1. 把游戏文件夹`File`里的`version.zip`移动出来，重上游戏下载数据`Fildder`抓包。
2. 找到地址后主要是下载'vo_normal_girl_12.u'文件，`normal`代表日常，`12`代表角色编号，在换装可以看到顺序编号。'vo_story_girl_12'表示故事线的语音，看看文件名都能知道。
3. 用`AssetStudio`解包语音文件，全部提取出来，用`Advanced Renamer`把后缀批量删除，`wem`后缀才是正确的。

voice的文件夹是提取音频的文件，有6个文件
bnkextr.exe 解压.bnk文件，解压出来是.wem文件。
revorb.bat  批量把.wem文件转换成.ogg音频
ww2ogg.exe 	.web to .ogg
revorb.exe  把转换.ogg矫正
packed_codebooks_aoTuV_603.b
delwem.bat  删除.web文件

1.复制出你需要解压的Vo_Normal_xxxx.bnk文件，用bnkextr.exe 打开，拖去bnkextr.exe 就可以了。
2.打开revorb.bat自动完成转换，再回车一次。如果转换出来的音频有不正常，就是少运行了一步。
3.可以运行delwem.bat  删除.web文件。



2020.3.9
\Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\English(US) 目录下是人物对话配合，好像不是Live2d的音频
\Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\  目录下是游戏音乐，L2D.bnk是Live2d语音，好像只加载游戏界面人物的语音。
如果转换wem显示Parse error: expected 0x42 fmt if vorb missing的错误，表示不支持此文件转换。
建议还是录屏提取Live2d语音简单粗暴。

2020.4.26
更新音频提取方法