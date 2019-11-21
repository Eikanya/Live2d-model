双生视界:女仆咖啡枪
雙生視界：少女咖啡槍
Girl Cafe cancer
ガールカフェガン


配置模型推荐用Live2DViewerEX，比较容易配置。

Live2d模型提取和语音提取方法

Live2d模型提取参考：https://www.perfare.net/1564.html。
模型已经提取出来了。

语音提取方法
音频文件在手机存储 \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android (日服)
国服的把jp.Marvelous.girlcafegun换成有bilibili的
人物语音在手机存储  \Android\data\jp.Marvelous.girlcafegun\files\AutoAudio\Android\English(US)
文件Vo_Normal开头的是人物语音，有可能不完整，可能是好感动不够吧，解压应该有30+音频.(确实需要的可以在那9000+的音频里面找，做听力练习吧)

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

我也没有提取全部角色的音频，Vo_Normal_xxxx.bnk里有的角色的文件太小，音频不全。
-----------------

提取出来的模型和音频自己配置吧，虽然有点麻烦，记得她们是你的老婆，坚持到最好。
基本每个角色都有一个裸体的模型。可以打开texture看看图片，看到奶子是单独的（比如泳装的模型），把胸罩用ps等软件用橡皮擦擦去，变成了色图，
会板绘的可以自己ghs。