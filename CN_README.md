# 原神资源
角色贴图合集

## 使用说明
 1. 下载任何人物贴图
 2. 在 [GIMP](https://www.gimp.org/) 中打开
 3. 选中主图层, 右键点击并选择添加图层蒙版
>![select add layer mask](https://i.imgur.com/yHC66Fd_d.webp?maxwidth=760&fidelity=grand)
 4. 勾选第四项并点击确认
>![](https://i.imgur.com/6LelrEy_d.webp?maxwidth=760&fidelity=grand)
 5. 用填充工具点击图片，确保颜色为白色，不透明度在百分之1-2
 6. 从图层切换到频道面板
 7. 隐藏Alpha通道，并选中Alpha通道
  **一定要选中Alpha通道**
 >![Make Sure Alpha is selected](https://i.imgur.com/2t5FcUP_d.webp?maxwidth=760&fidelity=grand)
 8. 现在就可以编辑图片了
 9. 导出图片为png格式
 10. 使用 [ModelChanger](https://github.com/portra400nc/ModelChanger) 或脚本替换贴图

## FAQ 
> Q: 这么多文件夹，我该用哪个？

A: 目前只有 BodyDiffuse, FaceDiffuse, 和 HairDiffuse 文件夹里的贴图可以在游戏内被替换

BodyDiffuse 为主材质
FaceDiffuse 为脸部材质
HairDiffuse 为头发材质

LightMap 和 ShadowRamp 现在无法导入游戏