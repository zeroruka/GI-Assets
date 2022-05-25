
[中文](https://github.com/zeroruka/GI_Textures/blob/main/CN_README.md) | English
# GI Textures
A collection of Genshin Character Texture files for modding.


## Guide
### Method 1 (recommended for testing)
 1. Download any texture you want to modify
 2. Open in [GIMP](https://www.gimp.org/)
 3. Select main layer, right click and select add layer mask
>![select add layer mask](https://i.imgur.com/yHC66Fd_d.webp?maxwidth=760&fidelity=grand)
 4. Choose Transfer layer's alpha channel and add mask.
> ![](https://i.imgur.com/6LelrEy_d.webp?maxwidth=760&fidelity=grand)
 5. Use the bucket fill tool and click on the canvas. Make sure fill colour is white, and opacity is 1-2%
 6. Switch from Mask back to picture in Layers tab, and then switch over from Layers tab to Channels tab.
 7. Hide the Alpha channel and deselect Alpha channel


  **Make sure Alpha channel is not selected as shown below**
>![Make Sure Alpha is not selected](https://i.imgur.com/2t5FcUP_d.webp?maxwidth=760&fidelity=grand)
 8. Now you can edit the image. 
 9. Export the edited image as png, or overwrite the existing file.
 10. Load texture into genshin using [ModelChanger](https://github.com/portra400nc/ModelChanger) or Scripts

### Method 2 (better for deploying and lightmap)
**Setting up SpecialK**

1. Download SpecialK Global Injector (SKIF) [here](https://wiki.special-k.info/SpecialK/Global)
2. Run SpecialK as admin (***Important***)
3. Add Genshin to Game Library
4. Start Genshin from SpecialK launcher *(note: it might take a few tries to succesfully inject SpecialK)*
5. Press ctrl + shift + backspace to open SpecialK menu
6. Change sRGB bypass from Passthrough to Strip
>![enter image description here](https://i.imgur.com/gkqZibH_d.webp?maxwidth=760&fidelity=grand)
7. Open 'Render Mod Tools' to see all textures for dumping. 


**Making textures**

Since SpecialK uses .dds format, GIMP could not be used. We will use "Paint .NET" instead

1. Download Paint .NET [here](https://www.dotpdn.com/files/paint.net.4.3.10.install.anycpu.web.zip)
2. Download and install the following plugins: [DDS File Type Plus](https://forums.getpaint.net/topic/111731-dds-filetype-plus-04-11-2022/) and [Modify Channels](https://forums.getpaint.net/topic/110805-modify-channels-v111-2022-03-07/)
3.  Follow [this](https://steamcommunity.com/sharedfiles/filedetails/?id=1491783680) guide to dump any game texture that you want to modify. Jump to Get Textures section of the guide.
4. Modify textures to your likings, save files in the corresponding formats below and make sure to turn on 'Generate Mip Map'
> Diffuse textures --> BC7 (sRGB, DX 11+)

> Lightmaps --> BC7 (Linear, DX 11+)
5. Continue following [this](https://steamcommunity.com/sharedfiles/filedetails/?id=1491783680) guide once you have finished editing your textures.


## Important notes (*pls read*)

1. If you use Method 1, ModelChanger/UnityExplorer does not currently support replacing lightmaps. Only Method 2 will be able to replace lightmaps.
2. SpecialK can be loaded simultaneously with Melon. There should be no conflicts.
3. SpecialK is better than UnityExplorer at changing textures, however SpecialK cannot import models.
4. SpecialK is more suited for deploying textures since it requires restart of game to load new changes to textures while UnityExplorer doesn't.
5. SpecialK automatically replaces textures, therefore teleporting to a waypoint does not affect modded textures.
6. SpecialK uses .dds format instead of png


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=zeroruka/GI_Textures&type=Date)](https://star-history.com/#zeroruka/GI_Textures&Date)

