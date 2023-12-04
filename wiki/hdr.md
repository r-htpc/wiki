# HDR Setup Guide

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

This setup guide is only for HDR10 passthrough. High-end tonemapping is not discussed here. Dolby Vision/HDR10**+** is not discussed here as **no passthrough options exist** on PC. Read our [HDR section](/htpc-wiki/faq#wiki_what_is_hdr_video_and_what_do_i_need_to_take_advantage_of_it.3F) in the Wiki FAQ for detailed information and requirements.  
We assume your display, video chain and media player have already been configured/calibrated properly for non-HDR content before you venture into the HDR setup below. If not, you are urged to follow the setup sections in the [Video Setup](/htpc-wiki/video#wiki_setup) wiki page first.  
You are **strongly urged** to test out the simple setups below before potentially moving onto the advanced ones.  

## WINDOWS

### **Common settings**

* *Requirements:*

 TV/Projector: HDMI >= 2.0/DisplayPort >= 1.3, HDR10, 10-bit panel, [VESA DisplayHDR](https://displayhdr.org/) >= 600

 Windows 10: version >= 1803  (Settings app -> System -> About)

* *TV/Projector settings:*  

 ONLY display connected to the system before configuration  

 GPU connected to display's HDMI >= 2.0/DisplayPort >= 1.3 port  

 UHD Deep Color/Input Signal Plus turned On for your display's HDMI port. Setting name dependent on TV mfgr.  

 Black Level to Full/Normal (if available)  

 Colorspace/Input Level/Range to RGB Full/Expanded/Enhanced/0-255 (if available)  

 
* *GPU settings:*  
* Intel  

   *Intel Graphics Control Panel/Command Center app ->*  

     -- Display -> Resolution/General Settings ->  

     Resolution: 3840x2160  

     Refresh: 24/30/60Hz  

     -- Display -> Color/Color Settings ->  

     Desktop color depth: Highest (32-bit)  

     -- Video -> Color Enhancement -> Input Range -> Driver Settings -> Full Range  

* NVIDIA  

   *Nvidia Control panel app ->*  

   -- Manage 3D Settings (>= RTX 20xx) -> Program Settings -> Select a program: <your media player> -> Vertical Sync: ON, Low Latency Mode: OFF, Power Managment Mode: Prefer Max/Adaptive/Normal  

   -- Display ->  

    ---- Change Resolution/Adjust desktop color settings:  

     Resolution: 3840x2160  

     Refresh: 24/30/60Hz  

     Desktop color depth: Highest (32-bit)  

     Output color depth: 8 bpc  

     Output color format: RGB  

     Output dynamic range: Full  

* AMD  

   *Windows ->*  

   -- [Change Resolution/Refresh Rate](https://www.amd.com/en/support/kb/faq/dh2-005#faq-Display-Resolution)  

    Resolution: 3840x2160  

    Refresh: 30/60Hz  

   *AMD Radeon Settings app ->*  

    -- Display ->  

     Color depth: 8 bpc  

     Pixel format: RGB/YCbCr 4:4:4 Full  

     Radeon FreeSync: Disabled (create an app profile for your video player if you don't want to disable this globally)  

    -- Graphics -> Enhanced Sync: Disabled  

## Local Content

### **Kodi 20 Nexus** (official)

Simple, HDR passthrough, tonemapping.  

* *Requirements:*  

  Common settings above  

  Install Kodi: >= 20 [download](https://mirrors.kodi.tv/releases/windows/win64/)  

* *Windows 10 settings:*  

  Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> Off  

*  *Kodi settings:*  

   *Kodi app ->*  

   -- Settings -> Player  

    ---- Use HDR display capabilities: ON  

* *Test*  

   *Kodi app ->*  

   Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **VLC**

Simple, HDR passthrough.  

* *Requirements:*  

  Common settings above  

  Install VLC: >= 3.0.8 [download](https://www.videolan.org/vlc/)  

* *Windows settings:*  

  Activate HDR

  Start -> Settings -> System -> Display -> Play HDR games and apps: On / Use HDR: On (Wording depends on Windows version)  

  Start -> Settings -> System -> Display -> Windows HD Color settings -> Stream HDR Video: On  

* *VLC settings:*  

   *Start -> VideoLAN -> VLC app ->*  

     Tools -> Preferences -> Video -> Output -> Automatic or OpenGL for Windows  

     Tools -> Preferences -> Input / Codecs -> Hardware-accelerated decoding: NOT Disable  

* *Test*  

   *VLC app ->*  

   Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **MPC-BE + MPC Video Renderer**

Simple, HDR passthrough, tonemapping and upscaling.  

* *Requirements:*  

  Install MPC-BE: [download](https://github.com/Aleksoid1978/MPC-BE/releases)  
  -- Install options: Default Installation + "MPC Video Renderer" option checked  

* *Windows 10 settings:*  

  Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> Off  

* *MPC-BE settings:*  

  *MPC-BE app ->*  

   -- View -> Options ->  

    --- Video -> Video Renderer -> MPC Video Renderer  
    ---- Properties  
    ----- Use Direct3D 11: checked (win 8+)  
    ----- HDR: Passthrough to display: checked (uncheck to tonemap to SDR)  
    ----- HDR: Convert to SDR: unchecked (check to tonemap to SDR)  
    ----- HDR: Auto display: used for fullscreen/always used  
    ----- OPTIONAL: Chroma/Upscaling. NOTE: To use these, you must uncheck the four DXVA2/D3D11 video processors. GPU usage will increase as you go down the list of scaling options.  
    ----- OPTIONAL: Downscaling. NOTE: To use this, you must uncheck "Use for Resizing". GPU usage will increase as you go down the list of scaling options.  

    --- Internal Filters -> Video Decoders  
    ---- Video decoder configuration  
    ----- Preferred Decoder: D3D11 (win 8+) or DXVA2 (win 7)  
    ----- Adapter: Your_GPU_Device  
    ----- RGB output levels: PC (0-255) (see VIDEO setup guide if not sure)  

* *Test*  

   *MPC-BE app ->*  

     Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests) and press Ctrl+J to show stats. If "Times" stats are >= 35ms you're doing too much processing (like upscaling/tonemapping). If "Frames" shows significant skipped frames, your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **MPC-HC/MPC-BE + madVR**

Advanced, more powerful tonemapping, upscaling and processing than using MPC Video Renderer, but more complicated.  

* *Requirements:*  

  MPC-HC: Install K-Lite Codec Pack FULL: [download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm)  
  -- Install options: Normal, MPC-HC, Essentials  
  MPC-BE: Install MPC-BE: [download](https://github.com/Aleksoid1978/MPC-BE/releases), then Install K-Lite Codec Pack FULL: [download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm)  
  -- K-lite install options: No, Normal, MPC-BE, Essentials  

* *Windows 10 settings:*  

  Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> Off  

* *LAV Filters settings:*  

   *Start -> K-lite Codec Pack -> LAV Video app ->*  

   -- Hardware decoder to use -> D3D11 (win 8+) or DXVA2 (copy-back)  

   -- Hardware device to use -> Your_GPU_Device (leave on Auto with D3D11)  

   -- Dithering mode -> Ordered dithering  

   *Start -> K-lite Codec Pack -> LAV Audio app ->*  

   -- Enable "Bitstreaming" for the codecs your sound system supports decoding (see Audio wiki page for more details)  


* *madVR settings:*  

   *Start -> K-lite Codec Pack -> madVR app ->*  

   -- Devices -> Your_Display_Device ->  

    ---- properties -> PC levels 0-255, bitdepth: 10 bit or higher  

    ---- calibration -> this display is already calibrated  

    ---- display modes -> switch to matching display mode..when playback starts  

    ---- display modes -> list all display..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  

    ---- HDR -> passthrough HDR content to the display, send HDR metadata to the display  

   -- Rendering -> general settings ->  

    ---- Enable delay playback start.., automatic fullscreen exclusive mode, use Direct3D 11 for presentation  

    ---- Increase CPU/GPU queue size (if frame drops/stuttering occur)  

   -- Rendering -> dithering -> ordered dithering (unless you have dedicated GPU, see settings section below)  

   -- Scaling Algorithms ->  

    ---- Chroma Upscaling -> Bilinear (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Downscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Upscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

* *MPC-HC/BE settings:*  

  *MPC-HC/BE app ->*  

   -- View -> Options ->  

    ---- MPC-HC: Playback -> Output -> Directshow Video -> madVR  

    ---- MPC-BE: Video -> Video Renderer -> madVR  

    ---- External Filters -> Add Filter... -> Add LAV Audio Decoder, LAV Splitter, LAV Splitter Source, LAV Video Decoder. Set all to "prefer".  

* *Test*  

   *MPC-HC/BE app ->*  

     Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 35ms, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

* *Update MadVR* (OPTIONAL)  

     If you want newer, beta madVR features, [download madVR beta](http://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **Kodi + MPC-HC + madVR**

Advanced, current way to integrate madVR into Kodi for passthrough, tonemapping, and upscaling.  

* *Requirements:*  

  Install Kodi: >= 17.6 [download](https://kodi.tv/download)  

  Install K-Lite Codec Pack FULL: [download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm)  
   -- Install options: Normal, MPC-HC, Essentials  

  (OPTIONAL) Install XySubFilter (64-bit) (subtitle renderer): [download](http://forum.doom9.org/showthread.php?t=168282)  

* *Windows 10 settings:*  

  Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> Off  

* *madVR settings:*  

   *Start -> K-lite Codec Pack -> madVR app ->*  

   -- Devices -> Your_Display_Device ->  

    ---- properties -> PC levels 0-255, bitdepth: 10 bit or higher  

    ---- calibration -> this display is already calibrated  

    ---- display modes -> switch to matching display mode..when playback starts  

    ---- display modes -> list all display..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  

    ---- HDR -> passthrough HDR content to the display, send HDR metadata to the display  

   -- Rendering -> general settings ->  

    ---- Enable delay playback start.., automatic fullscreen exclusive mode, use Direct3D 11 for presentation  

    ---- Increase CPU/GPU queue size (if frame drops/stuttering occur)  

   -- Rendering -> dithering -> ordered dithering (unless you have dedicated GPU, see settings section below)  

   -- Scaling Algorithms ->  

    ---- Chroma Upscaling -> Bilinear (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Downscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Upscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

* *MPC-HC settings:*  

  *Start -> K-lite Codec Pack -> Media Player Classic app ->*  

   -- View -> Options ->  

    ---- Player -> Enable "Remember File Position"  

    ---- Player -> Keys -> "Stop" & "Exit" commands -> Set to same key (so pressing it in Kodi will exit back to Kodi interface)   

    ---- Playback -> Output ->  

     ------ Directshow Video -> madVR  

     ------ Audio Renderer: SaneAR Audio Renderer  

     ------ (OPTIONAL) Subtitles -> Subtitle renderer: XySubFilter  

    ---- Playback -> Fullscreen -> Enable "Hide controls in fullscreen", "Hide Docked Panels"  

    ---- Internal Filters -> Audio Renderer -> Options -> Enable "Exclusive Mode"  

    ---- Internal Filters -> Internal LAV Filters Settings -> Video Decoder  

     ------ Hardware decoder to use -> D3D11 (win 8+) or DXVA2 (copy-back)  

     ------ Hardware device to use -> Your_GPU_Device (leave on Auto with D3D11)  

     ------ Dithering mode -> Ordered dithering  

    ---- Internal Filters -> Internal LAV Filters Settings -> Audio Decoder

     ------ Enable "Bitstreaming" for the codecs your sound system supports decoding (see Audio wiki page for more details)  

    ---- Internal Filters -> Internal LAV Filters Settings -> Splitter Decoder (OPTIONAL)  

   *Windows: Create text file: C:\Users\YOUR_USERNAME\AppData\Roaming\Kodi\userdata\playercorefactory.xml with content:*  

`<playercorefactory>`  
`<players>`  
`<player name="MPC-HC" type="ExternalPlayer" audio="false" video="true">`  
`<filename>C:\YOUR\SPECIFIC\PATH\TO\MPC-HC\mpc-hc64.exe</filename>`  
`<args>"{1}" /fullscreen /close</args>`  
`<hidexbmc>false</hidexbmc>`  
`<hideconsole>false</hideconsole>`  
`<warpcursor>none</warpcursor>`  
`</player>`  
`</players>`  
`<rules action="prepend">`  
`<rule filetypes="mkv|avi|divx|ogm|mp4|mov|m4v|flv|m2v|mpeg|mpg|mts|m2ts|vob|bdmv|iso" player="MPC-HC">`  
`<rule protocols="http|https" player="MPC-HC"/>`  
`<rule protocols="daap|rtv|rtsp|rtmp|rtmpe|rtsp|mms|rtp|pvr" player="VideoPlayer"/>`  
`</rule>`  
`</rules>`  
`</playercorefactory>`  

* *(ALTERNATIVE) MPC-BE settings:*  

   -- Install MPC-BE after K-lite Codec Pack

   *Start -> K-lite Codec Pack -> LAV Video app ->*  

   -- Hardware decoder to use -> D3D11 (win 8+) or DXVA2 (copy-back)  

   -- Hardware device to use -> Your_GPU_Device (leave on Auto with D3D11)  

   -- Dithering mode -> Ordered dithering  

   *Start -> K-lite Codec Pack -> LAV Audio app ->*  

   -- Enable "Bitstreaming" for the codecs your sound system supports decoding (see Audio wiki page for more details)  

  *MPC-BE app ->*  

   -- View -> Options ->  

    ---- Player -> Enable "Remember File Position"  

    ---- Player -> Keys -> "Stop" & "Exit" commands -> Set to same key (so pressing it in Kodi will exit back to Kodi interface)   

    ---- Video -> Video Renderer -> madVR  

    ---- Playback -> Disable "Default track preference"  

    ---- (OPTIONAL) Subtitles -> Subtitle renderer: XySubFilter  

    ---- External Filters -> Add Filter... -> Add LAV Audio Decoder, LAV Splitter Source, LAV Video Decoder. Set all to "prefer".  

   *Windows: Create text file: C:\Users\YOUR_USERNAME\AppData\Roaming\Kodi\userdata\playercorefactory.xml with content:*  

`<playercorefactory>`  
`<players>`  
`<player name="MPC-BE" type="ExternalPlayer" audio="false" video="true">`  
`<filename>C:\YOUR\SPECIFIC\PATH\TO\MPC-BE\mpc-be64.exe</filename>`  
`<args>"{1}" /fullscreen /close</args>`  
`<hidexbmc>false</hidexbmc>`  
`<hideconsole>false</hideconsole>`  
`<warpcursor>none</warpcursor>`  
`<playcountminimumtime>1140</playcountminimumtime>`  
`</player>`  
`</players>`  
`<rules action="prepend">`  
`<rule filetypes="mkv|avi|divx|ogm|mp4|mov|m4v|flv|m2v|mpeg|mpg|mts|m2ts|vob|bdmv|iso" player="MPC-BE">`  
`<rule protocols="http|https" player="MPC-BE"/>`  
`<rule protocols="daap|rtv|rtsp|rtmp|rtmpe|rtsp|mms|rtp|pvr" player="VideoPlayer"/>`  
`</rule>`  
`</rules>`  
`</playercorefactory>`  

* *Test*  

   *Kodi app ->*  

    Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 35ms, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

* *Update MadVR* (OPTIONAL)  

     If you want newer, beta madVR features, [download madVR beta](http://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **DSPlayer Kodi + madVR**

Advanced, old way to integrate madVR into Kodi for passthrough, tonemapping, and upscaling. Can't use Kodi past v17.6  

* *Requirements:*  

  Common settings above  

  Install K-Lite Codec Pack FULL: [download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm)  
  -- Install options: Normal, MPC-HC, Essentials  
  Install DSPlayer Kodi: >= 17.6 [download](https://forum.kodi.tv/showthread.php?pid=1972183#pid1972183)  

* *Windows 10 settings:*  

  Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> Off  

* *madVR settings:*  

   *madVR app ->*  

   -- Devices -> Your_Display_Device ->  

    ---- properties -> PC levels 0-255, bitdepth: 10 bit or higher  

    ---- calibration -> this display is already calibrated  

    ---- display modes -> switch to matching display mode..when playback starts  

    ---- display modes -> list all display..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  

    ---- HDR -> passthrough HDR content to the display, send HDR metadata to the display  

   -- Rendering -> general settings ->  

    ---- Enable delay playback start.., automatic fullscreen exclusive mode, use Direct3D 11 for presentation  

    ---- Increase CPU/GPU queue size (if frame drops/stuttering occur)  

   -- Rendering -> dithering -> ordered dithering (unless you have dedicated GPU, see settings section below)  

   -- Scaling Algorithms ->  

    ---- Chroma Upscaling -> Bilinear (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Downscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

    ---- Image Upscaling -> Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  

*  *Kodi settings:*  

   *Kodi app ->*  

   -- Settings -> Player Settings -> DSPlayer ->  

    ---- Helper: Create example player rule (click) -> Yes  

    ---- Video Renderer: madVR  

    ---- Audio Renderer: Internal Audio Renderer (SaneAR)  

    ---- Filters management: Internal filters  

    ---- Video Decoder ->  

    ------ Enable System Tray Icon: On  

    ------ Hardware decoder to use: D3D11  

    ---- Audio Decoder (OPTIONAL: for bitstreaming) ->  

    ------ Enable System Tray Icon: On  

    ------ Bitstreaming <codec>: On  

* *Test*  

   *Kodi app ->*  

     Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 35ms, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

* *Update MadVR* (OPTIONAL)  

     If you want newer, beta madVR features, [download madVR beta](http://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **Plex HTPC**

Simple, HDR Passthrough or Tonemapping  

*  *Requirements:*  
  Common settings above  
  Install Plex HTPC: >= 1.16 [download](https://www.plex.tv/media-server-downloads/#plex-app)  
 *Notes:*  
  If HDR is not configured as per below, HDR will be tonemapped to SDR. Available for Windows, Linux and Mac.  
*  *Plex HTPC settings:*  

    *Plex HTPC app->*  

   -- Settings -> Video -> Enable HDR Switching: Checked  
   -- Settings -> Video -> HDR Metadata Passthrough: Checked  

* *Test*  

   *Plex HTPC app ->*  

   Play a [test HDR video](/htpc-wiki/hdr#wiki_hdr_tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper PC/TV hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

&nbsp;
 
### **Plex Media Player (old)**

Simple, Tonemapping  

*  *Requirements:*  

  Common settings above  

  Plex Media Player 2.x  

 *Notes:*  

  HDR is not currently passed through; It is tonemapped to SDR. Available for Windows, Linux and Mac.  

*  *Plex Media Player settings:*  

    None  

## Streaming Content (Netflix, Youtube, etc..)

* *Requirements:*  

  Common settings above  

  Supported Web Browsers/Apps: Microsoft Edge (Netflix/Youtube), Microsoft Store app (Netflix), Google Chrome (Youtube)  

  Required Software: Microsoft Store [HEVC Extension](https://www.microsoft.com/en-us/p/hevc-video-extensions/9nmzlz57r3t7) (Netflix)  

* *Windows settings:*  

  Activate HDR. HDR must be turned on before viewing content; it will not switch to hdr mode automatically like local players. You can use the "Win + Alt + B" shortcut to turn on/off HDR in windows, subsequently.  

  Start -> Settings -> System -> Display -> Play HDR games and apps: On / Use HDR: On (Wording depends on Windows version)  

  Start -> Settings -> System -> Display -> Windows HD Color settings -> Stream HDR Video: On  

## ANDROID

### **Common Settings**

* *Requirements:*  

 TV/Projector: HDMI >= 2.0/DisplayPort >= 1.3, HDR10, 10-bit panel, [VESA DisplayHDR](https://displayhdr.org/) >= 500  

* *TV/Projector settings:*  

 GPU Connected to HDMI >= 2.0/DisplayPort >= 1.3 port  

 UHD Deep Color/Input Signal Plus turned On for your HDMI port. Setting name dependent on TV mfgr.  

## HDR Tests

[Our HDR10 Test Videos/Patterns](https://drive.google.com/uc?id=19i_laf6vloxzLic6qOArXt0fLvCpc_qo) - For Basic HDR video calibration  
[Mehanik's Full HDR10 Test Videos/Patterns](https://drive.google.com/drive/folders/1m4IBq0euAxamL9ePgfdFuf8_5nLcRwHA) - For Advanced HDR video calibration  
[Ideal 4K HEVC HDR10 test](https://4kmedia.org/samsung-hdr-picture-quality-uhd-4k-demo/) - High UHD Blu-Ray bitrate - 4k, HEVC, HDR10, 50-90Mbps, 10-bit, 30fps, mp4  

## MADVR PERFORMANCE SETTINGS PER GPU

WARNING: These settings are for more intensive image processing/scaling that is NOT necessary for just HDR passthrough.  
The settings for the corresponding GPU families below are a little conservative so you don't have to spend hours wasting your time with stuttering due to high rendering times and diminishing returns.  
This doesn't mean that they're not gpu intensive; they most certainly are. Test with the default settings before changing to any of these.  
If you can't handle the GPU load/noise/heat these settings produce, turn them down or go back to the madvr Bilinear defaults.  

GPU|IMAGE UPSCALING|IMAGE DOUBLING|IMAGE DOWNSCALING|CHROMA UPSCALING|DITHERING
:--|:--|:--|:--|:--|:--
Intel UHD >= 6xx|DXVA2|NA|DXVA2|BiCubic 75+AR|random
AMD Ryzen Vega xx|Cubic/Lanczos|NA|Cubic/Lanczos|BiCubic 75+AR|random
Nvidia GT 1030|Lanczos 3-tap+AR|NA|Lanczos 3-tap+AR|BiCubic 75+AR|random
Nvidia GTX 960/1050/1050 Ti|Lanczos 4-tap+AR|NA|SSIM 1D+LL+AR|Lanczos 3-tap+AR|random
Nvidia GTX 1650|Lanczos 4-tap+AR|Super-XBR|SSIM 1D+LL+AR|Lanczos 3-tap+AR|random
Nvidia GTX 1650 Super|Lanczos 4-tap+AR|NGU Standard Luma Low|SSIM 1D+LL+AR|Jinc+AR|Error Diff. #1
Nvidia GTX 970/1060|Jinc|NGU Standard Luma Med|SSIM 1D+LL+AR|Jinc+AR|Error Diff. #1
Nvidia GTX 980/1070/1660/1660 Super/1660 Ti/3050|Jinc|NGU Standard Luma High|SSIM 1D+LL+AR|NGU Standard Med|Error Diff. #2
Nvidia GTX 1080/RTX 2060|Jinc|NGU Sharp Luma High|SSIM 1D+LL+AR|NGU Standard High|Error Diff. #2
Nvidia GTX >= 1080Ti/RTX 2070|Jinc|NGU Sharp Luma Very High|SSIM 1D+LL+AR|NGU Standard High|Error Diff. #2
AMD RX 5xx|Jinc|NGU Standard Luma Low (RX 570/580)|SSIM 1D+LL+AR|super-xbr 100+AR|Error Diff. #2
AMD RX 56xx - 66xx|Jinc|NGU Standard Luma High|SSIM 1D+LL+AR|NGU Standard High|Error Diff. #2
AMD RX >= 67xx|Jinc|NGU Standard Luma Very High|SSIM 1D+LL+AR|NGU Standard High|Error Diff. #2
