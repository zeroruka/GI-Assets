中文 | [English](https://github.com/zeroruka/GI_Textures)
# 原神资源
角色贴图合集

## 使用说明
### 方法一 （适合测试贴图）
 1. 下载任何人物贴图
 2. 在 [GIMP](https://www.gimp.org/) 中打开
 3. 选中主图层, 右键点击并选择添加图层蒙版
>![select add layer mask](https://i.imgur.com/yHC66Fd_d.webp?maxwidth=760&fidelity=grand)
 4. 勾选第四项并点击确认
>![](https://i.imgur.com/6LelrEy_d.webp?maxwidth=760&fidelity=grand)
 5. 用填充工具点击图片，确保颜色为白色，不透明度在百分之1-2
 6. 在图层面板里从蒙版换回主图片，然后从图层切换到频道面板
 7. 隐藏Alpha通道，并取消选中Alpha通道


  **一定不要选中Alpha通道如下**
 >![Make Sure Alpha is not selected](https://i.imgur.com/2t5FcUP_d.webp?maxwidth=760&fidelity=grand)
 8. 现在就可以编辑图片了
 9. 导出图片为png格式
 10. 使用 [ModelChanger](https://github.com/portra400nc/ModelChanger) 或脚本替换贴图

### 方法二 （支持修改lim）
**配置 SpecialK**

1. 在[这里](https://wiki.special-k.info/SpecialK/Global)下载 SpecialK Global Injector (SKIF) 
2. 以管理员身份运行 SpecialK (***重要***)
3. 添加原神到 SpecialK 的游戏库
4. 从 SpecialK 里启动原神 *(注: 可能需要多次尝试才能成功)*
5. 按 ctrl + shift + backspace 打开 SpecialK 菜单
6. 把 sRGB bypass 从 Passthrough 换到 Strip
>![enter image description here](https://i.imgur.com/gkqZibH_d.webp?maxwidth=760&fidelity=grand)
7. 打开 'Render Mod Tools' 查看所有游戏材质

**制作贴图**

因为 SpecialK 用的是 .dds 格式, 我们不能使用 GIMP， 所以要用到 "Paint .NET"

1. 在[这里](https://www.dotpdn.com/files/paint.net.4.3.10.install.anycpu.web.zip)下载 Paint .NET 
2. 下载并安装以下插件: [DDS File Type Plus](https://forums.getpaint.net/topic/111731-dds-filetype-plus-04-11-2022/) and [Modify Channels](https://forums.getpaint.net/topic/110805-modify-channels-v111-2022-03-07/)
3.  跟着[这个](https://steamcommunity.com/sharedfiles/filedetails/?id=1491783680)教程获取游戏dds格式贴图。阅读 Get Textures 部分.
4. 有了材质就可以编辑啦, 保存文件时要注意打开 'Generate Mip Map' 并保存文件为以下格式 
> Diffuse textures --> BC7 (sRGB, DX 11+)

> Lightmaps --> BC7 (Linear, DX 11+)
5. 继续阅读[这个教程](https://steamcommunity.com/sharedfiles/filedetails/?id=1491783680) Inject Texture 的部分


**更多详情在 [wiki](https://wiki.special-k.info/SpecialK) 上查看**
## 重要注意事项 (*仔细阅读*)

1. If you use Method 1, ModelChanger/UnityExplorer does not currently support replacing lightmaps. Only Method 2 will be able to replace lightmaps.
2. SpecialK can be loaded simultaneously with Melon. There should be no conflicts.
3. SpecialK is better than UnityExplorer at changing textures, however SpecialK cannot import models.
4. SpecialK is more suited for deploying textures since it requires restart of game to load new changes to textures while UnityExplorer doesn't.
5. SpecialK automatically replaces textures, therefore teleporting to a waypoint does not affect modded textures.
6. SpecialK uses .dds format instead of png

