**双生视界:女仆咖啡枪**
**雙生視界：少女咖啡槍**
**Girl Cafe cancer**
**ガールカフェガン**

**日服与2021.8.31停服。此live2d和spine资源不完整，如有需要请自行提取。spine动态在2dAnimation文件夹，就是氪金购买的皮肤**


配置模型推荐用Live2DViewerEX，比较容易配置。

**Live2d模型提取和语音提取方法

Live2d模型提取参考：[链接](https://www.perfare.net/1564.html)。
模型已经提取出来了。

语音提取方法：
**步骤**   
1.  把游戏文件夹`File`里的`version.zip`移动出来，重上游戏下载数据`Fildder`抓包。
2. 找到地址后主要是下载`vo_normal_girl_12.u`[下载](https://cdn-cafe2.xoyo.jp/seasun_jp/10114/Android/V529/Bundles/wwisedata/english(us)/vo_normal_girl_01.u) 文件, 音频文件`url`后缀`/Bundles/wwisedata/english(us)/vo_normal_girl_12.u`,
音频文件是下载到`wwisedata`文件夹然后解压到`audio/english(us)/`文件夹里，`normal`代表日常，`12`代表角色编号，在换装可以看到顺序号。`vo_story_girl_12`表示故事线的语音，看看文件名都能知道.注意：请求文件的文件名是小写
3. 用`AssetStudio`解包语音文件，全部提取出来，用`Advanced Renamer`把后缀批量删除，`wem`后缀才是正确的。
4. `bnk`文件用`bnkextr`提取，出来文件后缀是`wem`。如果提取不出来说明这文件不需要的。
5.  用`revorb.bat`批量把`.wem`文件转换成`.ogg`音频，在修正'.ogg'音频文件。
```
for %%f in (*.wem) do ww2ogg.exe %%f --pcb packed_codebooks_aoTuV_603.bin
pause 
for %%f in (*.ogg) do revorb.exe %%f 
pause

```

6.  删除多余的`.wem`文件，根目录`delwem.bat`。 
```
del *.wem

```

音频文件在手机存储 \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android (日服)
国服的把jp.Marvelous.girlcafegun换成有bilibili的
人物语音在手机存储  \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\English(US)
文件Vo_Normal开头的是人物语音。

1. 把游戏文件夹`File`里的`version.zip`移动出来，重上游戏下载数据`Fildder`抓包。
2. 找到地址后主要是下载'vo_normal_girl_12.u'文件，`normal`代表日常，`12`代表角色编号，在换装可以看到顺序编号。'vo_story_girl_12'表示故事线的语音，看看文件名都能知道。
3. 用`AssetStudio`解包语音文件，全部提取出来，用`Advanced Renamer`把后缀批量删除，`wem`后缀才是正确的。

voice的文件夹是提取音频的文件，有6个文件
- bnkextr.exe 解压.bnk文件，解压出来是.wem文件。
- revorb.bat  批量把.wem文件转换成.ogg音频
- ww2ogg.exe 	.web to .ogg
- revorb.exe  把转换.ogg矫正
- packed_codebooks_aoTuV_603.b
- delwem.bat  删除.web文件

1.复制出你需要解压的Vo_Normal_xxxx.bnk文件，用bnkextr.exe 打开，拖去bnkextr.exe 就可以了。
2.打开revorb.bat自动完成转换，再回车一次。如果转换出来的音频有不正常，就是少运行了一步。
3.可以运行delwem.bat  删除.web文件。





```
2020.3.9
\Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\English(US) 目录下是人物对话配合，好像不是Live2d的音频
\Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\  目录下是游戏音乐，L2D.bnk是Live2d语音，好像只加载游戏界面人物的语音。
如果转换wem显示Parse error: expected 0x42 fmt if vorb missing的错误，表示不支持此文件转换。
建议还是录屏提取Live2d语音简单粗暴。

2020.4.26
更新音频提取方法

4.28 更新
- 10qpt01__l2d_354.u
- 10qpt01__l2d_355.u
- 10qpt01__l2d_356.u
- 10qpt01__l2d_357.u
- sy3q__l2d_342.u
- ybxd0414__l2d_336.u
- ybxd0414__l2d_337.u
- ybxd0414__l2d_338.u
- ybxd0414__l2d_339.u

20.12.8
添加语音提取方法

21.5.22
更新角色语音