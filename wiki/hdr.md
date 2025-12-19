---
description: Information on configuring HDR and Upscaling on your HTPC, for multiple platforms and media players (MPC VR, MPC-HC, MPC-BE, madVR, Kodi, Plex, VLC, Potplayer)
keywords: [hdr, hdr10, madvr, mpc, tonemapping, kodi, plex, upscaling]
---

# HDR Setup Guide

<meta name="viewport" content="width=625, initial-scale=0.8">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->
 
## Overview
* This setup guide is only for HDR10 passthrough and simple tonemapping.
  - *Passthrough* refers to sending the HDR metadata to the display as-is, resulting in the display showing an HDR logo and doing its own brightness level tonemapping of the content based on the displays capabilities. This is ideal. 
  - *Simple tonemapping* refers to modifying the HDR metadata on the source device to fit inside the brightness and color range of the display. This is usually done for SDR or poorly-capable HDR displays. By default, this is done to SDR levels with a target brightness of 100 nits and the Rec. 709 [color space](https://r-htpc.github.io/wiki/video#video-metadatacolor-technologies). On some renderers below (like madVR/MPC VR) this nits value is configurable.
  - *Dynamic Tonemapping* refers to modifying the HDR metadata on the source device to adjust the brightness levels on a per-scene basis in an attempt to simulate HDR10+/Dolby Vision metadata. This requires a lot of processing and at least a mid-range GPU (see our [Components Guide](/wiki/components#gpusgraphics)). This method is not covered here.
* **Dolby Vision/HDR10+ is not discussed here as no stable passthrough options exist on a PC**. For basic [Profile 5/7M/8](/wiki/video#video-metadatacolor-technologies) support, either use [JRiver](https://jriver.com/) and it's own dynamic tonemapping with basic DV metadata to [HDR10](/wiki/video#video-metadatacolor-technologies), MPC Video Renderer in [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases) with static tonemapping to [HDR10](/wiki/video#video-metadatacolor-technologies), or read [this post](https://www.reddit.com/r/htpc/comments/1936n8g/dolby_vision_lldv_now_possible_on_windows_1011/) for other experimental support; otherwise buy a [Media Device](/wiki/sample-builds#specialized-dolby-vision--hdr10).  
* Read our [HDR section](/wiki/faq#what-is-hdr-video-and-what-do-i-need-to-take-advantage-of-it) of the Wiki FAQ for detailed information on PC hardware requirements.  
* This guide is for HT displays only. Neither monitors, nor multiple displays are officially supported here.  
* We assume your display, video chain and media player have already been configured/calibrated properly for **SDR/non-HDR** content before you venture into a **HDR** setup below. If not, you are urged to follow the setup sections in the [Video Setup Guide](/wiki/video) of the Wiki first.  
* You are **strongly urged** to test out the simple setups below before moving onto the advanced ones. Do **NOT** skip any steps or make changes to the settings below until you verify HDR is working. Only then should you go back and make changes specific to your setup.  

## Common Settings

### **Hardware**

* *Requirements:*
  * TV/Projector: HDMI >= 2.0/DisplayPort >= 1.3, HDR10, 10-bit panel, [OLED/Mini-LED TV Recommended](https://www.rtings.com/tv/tools/table/136186)
  * HTPC: [HDR-capable PC](/wiki/sample-builds#4k-hdr-players) / [Media Device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc)
  * Cables: [Premium/Ultra-Certified HDMI Cables](/wiki/components#video-cablesadapters)
* *TV/Projector settings:*  
  * Must be the **ONLY** display connected to the system before configuration  
  * GPU connected to display's HDMI >= 2.0/DisplayPort >= 1.3 port  
  * UHD Deep Color/Input Signal Plus/Enhanced turned On for your display's HDMI port (setting name dependent on TV mfgr)  
  * Black Level to Full/Normal (if available)  
  * Colorspace/Input Level/Range to RGB Full/Expanded/Enhanced/0-255 (if available)  
* *AV Receiver settings (if in-between PC and Display):*  
  * HDMI Format/4k Signal Format set to Enhanced

### **Software**

* *Windows:*  
  * *GPU settings:*  
    * Intel  
      * Intel Graphics Control Panel/Command Center app
        * **Settings location varies per app/driver version**
        * Display -> General -> Display Settings
          * Resolution: 3840x2160  
          * Refresh: 24/30/60Hz  
        * Display -> Genenal / Display -> Color/Color Settings  
          * Color Depth: BPC_8 (HDMI 2.0), BPC_10 (HDMI 2.1) / Highest (32-bit)
          * Color Format: [RGB](/wiki/video#setup-for-color-reproduction) 
        * Video -> Color Enhancement -> Input Range -> Driver Settings -> [Full Range](/wiki/video#setup-for-color-reproduction)  
    * NVIDIA  
      * Nvidia Control panel app
        * Manage 3D Settings (>= RTX 20xx) -> Program Settings -> Select a program: \<your media player\> -> Vertical Sync: ON, Low Latency Mode: OFF, Power Managment Mode: Prefer Max/Adaptive/Normal  
        * Display  
          * Change Resolution/Adjust desktop color settings:  
            * Resolution: 3840x2160  
            * Refresh: 24/30/60/120Hz  
            * Desktop color depth: Highest (32-bit)  
            * Output color depth: 8 bpc (HDMI 2.0/2.1 TMDS), 10 bpc (HDMI 2.1 FRL)  
            * Output color format: [RGB](/wiki/video#setup-for-color-reproduction)  
            * Output dynamic range: [Full](/wiki/video#setup-for-color-reproduction)  
    * AMD  
      * Windows
        * [Change Resolution/Refresh Rate](https://www.amd.com/en/support/kb/faq/dh2-005#faq-Display-Resolution)  
          * Resolution: 3840x2160  
          * Refresh: 30/60/120Hz  
      * AMD Radeon Settings app
        * Display
          * Color depth: 8 bpc (HDMI 2.0), 10 bpc (HDMI 2.1)  
          * Pixel format: [RGB/YCbCr 4:4:4 Full](/wiki/video#setup-for-color-reproduction)  
          * Radeon FreeSync: Disabled (create an app profile for your media player if you don't want to disable this globally)
          <!-- Graphics -> Enhanced Sync: Disabled -->
  * *Windows settings:*
    * Check Windows 1x version: OS build >= 17134 (Settings app -> System -> About)
    * Calibrate your display for HDR in Windows. *Windows 11:* [Windows App](https://support.microsoft.com/en-us/windows/calibrate-your-hdr-display-using-the-windows-hdr-calibration-app-f30f4809-3369-43e4-9b02-9eabebd23f19). *Windows 10:* Run Start->Calibrate Display Color 
* *LibreElec:*  
  * [4K/HDR](https://wiki.libreelec.tv/configuration/4k-hdr)
* *CoreElec:*  
  * [Display Settings](https://wiki.coreelec.org/coreelec:kodi_ce_sys_settings)
* *Linux Desktop:*  
  * Kubuntu 25.10
  * KDE Plasma 6.x + Wayland
* *Android-like/Roku:*  
  * [Nvidia Shield](https://www.nvidia.com/en-us/shield/support/shield-tv-pro/4k-hdr-dolby-vision-display-setup/) / [Fire TV](https://www.amazon.com/gp/help/customer/display.html?nodeId=G8GNX2B27JG726AH&ref_=hp_GHH5TUHA7677G4HJ_Dolby-Vision-or-High-Dynamic-R) / [Chromecast](https://support.google.com/chromecast/answer/10117046?hl=en&sjid=10251772960481040502-NC) / [Roku](https://support.roku.com/article/235168467)


## Local Content

### **Kodi**

Simple, HDR passthrough or tonemapping.  

* *Requirements:*  
  * Common settings above  
  * Install Kodi: >= 20 ([download](https://mirrors.kodi.tv/releases/windows/win64/)) app or [LibreElec](https://libreelec.tv/downloads/)/[CoreElec](https://coreelec.org/#install) OS  
* *Windows 1x settings:*  
  * Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> **Off**  
* *Kodi settings:*  
  * *Kodi app*  
    * Settings -> Player -> Videos
      * v21: Adjust display HDR mode: ON (*off to [tonemap](https://kodi.wiki/view/Video_playback) to SDR*)  
      * v20: Use display HDR capabilities: ON
    * *OPTIONAL*: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
* *Test*  
  * *Kodi app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **VLC**

Simple, HDR passthrough or tonemapping.  

* *Requirements:*  
  * Common settings above  
  * Install VLC: >= 3.0.8: ([download](https://www.videolan.org/vlc/))
* *Windows settings:*  
  * Activate HDR
    * *For static tonemapping to SDR*: Ignore this section
    * Start -> Settings -> System -> Display
      * Windows 10
        * Windows HD Color settings
          * Use HDR: On / Play HDR games and apps: On (Wording depends on Windows version)  
          * Stream HDR Video: On  
      * Windows 11
        * HDR
          * (Use) HDR: On  
          * HDR video streaming..: On  
* *VLC settings:*  
  * *VLC app*  
    * Tools -> Preferences
      * Video
        * Output: OpenGL video output for Windows
        * *For static tonemapping to SDR*: Show settings: All, Video->Output Modules->OpenGL (2nd one)->Tone-mapping algorithm->[Hable (standard)/Reinhard (bright)/Mobius (brighter)/Hard-clip (brightest)](https://imgur.com/6V99TYA)
      * Input / Codecs
        * Hardware-accelerated decoding: Direct3D11 (win 8/10/11) or DXVA (win 7)
      * *OPTIONAL*: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart VLC app*  
* *Test*  
  * *VLC app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **MPC-BE + MPC Video Renderer**

Simple, HDR passthrough, tonemapping and decent upscaling.  

* *Requirements:*  
  * Install MPC-BE: ([download](https://github.com/Aleksoid1978/MPC-BE/releases))  
    * Install options: Default Installation + "MPC Video Renderer" option checked  
* *Windows 1x settings:*  
  * Settings app -> System -> Display -> Use HDR/HDR and WCG/Play HDR.. -> **Off**  
* *MPC-BE settings:*  
  * *MPC-BE app*  
    * View -> Options
      * Video
        * Video Renderer: MPC Video Renderer  
          * Properties  
            * Use Direct3D 11: checked (win 8/10/11)  
            * HDR: Passthrough to display: checked (*unchecked to tonemap to SDR*)  
            * HDR: Convert to SDR: unchecked (*checked to tonemap to SDR*)  
            * HDR: Windows HDR: Allow turn on/off  
            * OPTIONAL: Chroma/Upscaling
              * NOTE: To use these, you must uncheck the four DXVA2/D3D11 video processors. GPU usage will increase as you go down the list of scaling options.
              * Chroma/Upscaling: [\<choose\>](/wiki/video#what-are-the-best-ways-for-scaling-video)
            * OPTIONAL: Downscaling
              * NOTE: To use this, you must uncheck "Use for Resizing".
              * Downscaling: \<choose\>
      * Internal Filters -> Video Decoders  
        * Video decoder configuration  
          * Preferred Decoder: 'D3D11, DXVA2' (win 8/10/11) or DXVA2 (win 7) 
          * Adapter: \<your_GPU_device\> 
          * RGB output levels: PC (0-255) (see VIDEO setup guide if not sure) 
      * *OPTIONAL*: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart MPC-BE app*  
* *Test*  
  * *MPC-BE app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests) and press Ctrl+J to show stats. If "Times" stats are >= 33ms for 30fps, you're doing too much processing (like upscaling/tonemapping). If "Frames" shows significant skipped frames, your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **MPC-HC/MPC-BE + madVR**

Advanced, more powerful dynamic tonemapping, high-end upscaling and processing than using MPC Video Renderer, but more complicated.  

<!-- ALTERNATIVE INSTALL METHOD 
* *Requirements:*  
  * MPC-HC/MPC-BE: 
    * MPC-HC: Install MPC-HC from exe ([download](https://github.com/clsid2/mpc-hc/releases))
    * MPC-BE: Install MPC-BE from installer: ([download](https://github.com/Aleksoid1978/MPC-BE/releases))
  * MadVR: Install madVR from stable zip ([download](http://madshi.net/madVR.zip))
    * Extract/copy madVR directory in zip to directory: %USERPROFILE%\
    * Go into extracted directory %USERPROFILE%\madVR, right-click on 'install.bat' script and click on Run as administrator option to install.
* *madVR settings:*  
  * Run %USERPROFILE%\madVR\madHcCtrl.exe program
    * devices
      * \<your_display_device\>
        * properties -> PC levels 0-255, bitdepth: 10 bit or higher  
        * calibration -> this display is already calibrated  
        * display modes (OPTIONAL - for refresh rate switching)
          * Enable: switch to matching display mode..when playback starts  
          * list all display modes..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  
        * HDR -> passthrough HDR content to the display, send HDR metadata to the display  
          * *ALT: For static tonemapping to SDR*: HDR -> let madVR decide + rendering->trade quality for..->don't measure HDR.. option checked
    * scaling algorithms
      * chroma upscaling
        * processing..: Bilinear (for more intensive scaling, see Performance settings section at the bottom)  
      * image downscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
      * image upscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
    * rendering
      * general settings
        * Enable: delay playback start.., enable automatic fullscreen exclusive mode, use Direct3D 11 for presentation  
        * **If** frame drops/stuttering occur while testing, increase CPU/GPU queue size here
      * dithering
        * algorithm: Ordered dithering (unless you have dedicated GPU, see settings section below)  
* *MPC-HC/BE settings:*  
  * *MPC-HC app*  
    * View -> Options
      * Playback -> Output
        * DirectShow Video: madVR  
      * Internal Filters -> Video Decoder  
        * Hardware Decoder to use: 'D3D11' (win 8/10/11) or DXVA2 (copy-back) (win 7) 
        * Hardware Device to use: \<your_GPU_device\> 
        * RGB output levels: PC (0-255) (see VIDEO setup guide if not sure) 
      * *OPTIONAL*: Audio: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart MPC-HC app*  
  * *MPC-BE app*  
    * View -> Options
      * Video
        * Video Renderer: madVR  
      * Internal Filters -> Video Decoders  
        * Video decoder configuration  
          * Preferred Decoder: 'D3D11, DXVA2' (win 8/10/11) or DXVA2 (win 7) 
          * Adapter: \<your_GPU_device\> 
          * RGB output levels: PC (0-255) (see VIDEO setup guide if not sure) 
      * *OPTIONAL*: Audio: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart MPC-BE app*  
-->

* *Requirements:*
  * *If you don't want to use the K-lite Codec Pack way to install, see the [Appendix](/wiki/hdr#appendix) section for the minimal MPC-HC/BE and madVR software config* 
  * MPC-HC: Install K-Lite Codec Pack FULL: ([download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm))  
    * Install options: Mode: Normal, Player: MPC-HC, Components: Essentials, Defaults for everything else
  * MPC-BE: Install MPC-BE: ([download](https://github.com/Aleksoid1978/MPC-BE/releases)), then Install K-Lite Codec Pack FULL: ([download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm))  
    * K-lite install options: Mode: Normal, Player: MPC-BE, Components: Essentials, Defaults for everything else  
* *Windows 1x settings:*  
  * Settings app -> System -> Display -> Use HDR/HDR and WCG/Play HDR.. -> **Off**  
  * Windows 11: Settings app -> System -> Display -> Color Profile -> Color Management -> Automatically manage color for apps.. -> **Off**  
* *LAV Filters settings:*  
  * *Start -> K-lite Codec Pack -> LAV Video app*  
    * Hardware decoder to use -> D3D11 (win 8/10/11) or DXVA2 (copy-back)  
    * Hardware device to use -> Automatic (Native), or if DXVA2 (copy-back), then \<your_GPU_device\>  
    * Dithering mode -> Ordered dithering  
  * *Start -> K-lite Codec Pack -> LAV Audio app ->*  
    * Enable "Bitstreaming" for the codecs your sound system supports decoding (see [Wiki:Audio Setup Guide](/wiki/audio#softwareos-setup) for more details)  
* *madVR settings:*  
  * *Start -> K-lite Codec Pack -> madVR app*  
    * devices
      * \<your_display_device\>
        * properties -> PC levels 0-255, bitdepth: 10 bit or higher  
        * calibration -> this display is already calibrated  
        * display modes (OPTIONAL - for refresh rate switching)
          * Enable: switch to matching display mode..when playback starts  
          * list all display modes..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  
        * HDR -> passthrough HDR content to the display, send HDR metadata to the display  
          * *ALT: For static tonemapping to SDR*: HDR -> let madVR decide + rendering->trade quality for..->don't measure HDR.. option checked
    * scaling algorithms
      * chroma upscaling
        * processing..: Bilinear (for more intensive scaling, see Performance settings section at the bottom)  
      * image downscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
      * image upscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
    * rendering
      * general settings
        * Enable: delay playback start.., enable automatic fullscreen exclusive mode, use Direct3D 11 for presentation  
        * **If** frame drops/stuttering occur while testing, increase CPU/GPU queue size here
      * dithering
        * algorithm: Ordered dithering (unless you have dedicated GPU, see settings section below)  
* *MPC-HC/BE settings:*  
  * *MPC-HC/BE app*  
    * View -> Options
      * MPC-HC  
        * Playback -> Output -> Directshow Video -> madVR  
        * External Filters -> Add Filter... -> Add LAV Audio Decoder, LAV Video Decoder. Set all to "prefer".  
      * MPC-BE  
        * Video -> Video Renderer -> madVR  
        * External Filters -> Add Filter... -> Add LAV Audio Decoder, LAV Splitter, LAV Splitter Source, LAV Video Decoder. Set all to "prefer".  
    * *Restart MPC-HC/BE app*  
* *Test*  
  * *MPC-HC/BE app*  
    *  Play a [test HDR video](/wiki/hdr#hdr-tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 33ms for 30fps, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  
* *Update MadVR* (OPTIONAL)  
  * If you want newer, beta madVR features, after validating your setup, [download madVR beta](https://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **Kodi + MPC-HC + madVR**

Advanced, current way to integrate madVR into Kodi for passthrough, dynamic tonemapping, and high-end  upscaling.  

* *Requirements:*
  * Install Kodi: >= 17.6: ([download](https://kodi.tv/download))
  * Install K-Lite Codec Pack FULL: ([download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm))
    * Install options: Normal, MPC-HC, Essentials
  * (OPTIONAL) Install XySubFilter (64-bit) (subtitle renderer): ([download](http://forum.doom9.org/showthread.php?t=168282))
* *Windows 1x settings:*
  * Settings app -> System -> Display -> Use HDR/HDR and WCG/Play HDR.. -> **Off**
  * Windows 11: Settings app -> System -> Display -> Color Profile -> Color Management -> Automatically manage color for apps.. -> **Off**  
* *madVR settings:*
  * *Start -> K-lite Codec Pack -> madVR app*  
    * devices
      * \<your_display_device\>
        * properties -> PC levels 0-255, bitdepth: 10 bit or higher  
        * calibration -> this display is already calibrated  
        * display modes (OPTIONAL - for refresh rate switching)
          * Enable: switch to matching display mode..when playback starts  
          * list all display modes..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  
        * HDR -> passthrough HDR content to the display, send HDR metadata to the display  
          * *ALT: For static tonemapping to SDR:* HDR -> let madVR decide + rendering->trade quality for..->don't measure HDR.. option checked
    * scaling algorithms
      * chroma upscaling
        * processing..: Bilinear (for more intensive scaling, see Performance settings section at the bottom)  
      * image downscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
      * image upscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
    * rendering
      * general settings
        * Enable: delay playback start.., enable automatic fullscreen exclusive mode, use Direct3D 11 for presentation  
        * **If** frame drops/stuttering occur while testing, increase CPU/GPU queue size here
      * dithering
        * algorithm: Ordered dithering (unless you have dedicated GPU, see settings section below)  
* *MPC-HC settings:*  
  * *Start -> K-lite Codec Pack -> Media Player Classic app ->*  
    * View -> Options
      * Player
        * Enable "Remember File Position" 
        * Keys
          * "Stop" & "Exit" commands -> Set to same key (so pressing it in Kodi will exit back to Kodi interface) 
      * Playback
        * Fullscreen
          * Enable "Hide controls in fullscreen", "Hide Docked Panels"  
        * Output
          * Directshow Video: madVR  
          * Audio Renderer: SaneAR Audio Renderer
          * (OPTIONAL) Subtitles -> Subtitle renderer: XySubFilter  
      * Internal Filters
        * Internal LAV Filters Settings
          * Video Decoder
            * Hardware decoder to use -> D3D11 (win 8/10/11) or DXVA2 (copy-back) 
            * Hardware device to use -> Automatic (Native), or if DXVA2 (copy-back), then \<your_GPU_device\>  
            * Dithering mode -> Ordered dithering
          * Audio Decoder
            * Enable "Bitstreaming" for the codecs your sound system supports decoding (see [Wiki:Audio Setup Guide](/wiki/audio#softwareos-setup) for more details)   
        * Audio Renderer
          * Options -> Enable "Exclusive Mode"
        * Splitter (OPTIONAL) 

* *Windows: Find file path to MPC-HC (usually C:\Program Files (x86)\K-Lite Codec Pack\MPC-HC64\mpc-hc64.exe) and Create text file: C:\Users\YOUR_USERNAME\AppData\Roaming\Kodi\userdata\playercorefactory.xml with contents of:*  

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
   * Install MPC-BE after K-lite Codec Pack
     * *Start -> K-lite Codec Pack -> LAV Video app ->*  
       * Hardware decoder to use -> D3D11 (win 8/10/11) or DXVA2 (copy-back)  
       * Hardware device to use -> Automatic (Native), or if DXVA2 (copy-back), then \<your_GPU_device\>  
       * Dithering mode -> Ordered dithering  
     * *Start -> K-lite Codec Pack -> LAV Audio app ->*  
       *  Enable "Bitstreaming" for the codecs your sound system supports decoding (see Audio wiki page for more details)  
     * *MPC-BE app ->*  
       * View -> Options
         * Player
           * Enable "Remember File Position" 
           * Keys
             * "Stop" & "Exit" commands -> Set to same key (so pressing it in Kodi will exit back to Kodi interface) 
         * Playback
           * Disable "Default track preference"
         * Video
           * Video Renderer: madVR  
         * Audio
           * Audio Renderer: MPC Audio Renderer
         * (OPTIONAL) Subtitles -> Subtitle renderer: XySubFilter  
         * External Filters
           * Add Filter... -> Add LAV Audio Decoder, LAV Splitter Source, LAV Video Decoder. Set all to "prefer".  

  * *Windows: Find file path to MPC-BE (usually C:\Program Files\MPC-BE x64\mpc-be64.exe) and Create text file: C:\Users\YOUR_USERNAME\AppData\Roaming\Kodi\userdata\playercorefactory.xml with contents of:*  

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
  * *Kodi app*
    * Play a [test HDR video](/wiki/hdr#hdr-tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 33ms for 30fps, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

* *Update MadVR* (OPTIONAL)
  * If you want newer, beta madVR features, after validating your setup, [download madVR beta](https://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **DSPlayer Kodi + madVR**

Advanced, OLD way to integrate madVR into Kodi for passthrough, tonemapping, and high-end upscaling. Can't use Kodi past v17.6, so not recommended vs MPC way.   

* *Requirements:*
  * Common settings above
  * Install K-Lite Codec Pack FULL: ([download](https://www.codecguide.com/download_k-lite_codec_pack_full.htm))
    * Install options: Normal, MPC-HC, Essentials
  * Install DSPlayer Kodi: >= 17.6: ([download](https://forum.kodi.tv/showthread.php?pid=1972183))
* *Windows 1x settings:*
  * Settings app -> System -> Display -> Use HDR/HDR and WCG/Play HDR.. -> **Off**
  * Windows 11: Settings app -> System -> Display -> Color Profile -> Color Management -> Automatically manage color for apps.. -> **Off**  
* *madVR settings:*
  * *Start -> K-lite Codec Pack -> madVR app*  
    * devices
      * \<your_display_device\>
        * properties -> PC levels 0-255, bitdepth: 10 bit or higher  
        * calibration -> this display is already calibrated  
        * display modes (OPTIONAL - for refresh rate switching)
          * Enable: switch to matching display mode..when playback starts  
          * list all display modes..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  
        * HDR -> passthrough HDR content to the display, send HDR metadata to the display  
          * ALT: For static tonemapping to SDR: HDR -> let madVR decide + rendering->trade quality for..->don't measure HDR.. option checked
    * scaling algorithms
      * chroma upscaling
        * processing..: Bilinear (for more intensive scaling, see Performance settings section at the bottom)  
      * image downscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
      * image upscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
    * rendering
      * general settings
        * Enable: delay playback start.., enable automatic fullscreen exclusive mode, use Direct3D 11 for presentation  
        * **If** frame drops/stuttering occur while testing, increase CPU/GPU queue size here
      * dithering
        * algorithm: Ordered dithering (unless you have dedicated GPU, see settings section below)  
* *Kodi settings:*  
  * *Kodi app*  
    * Settings
      * Player Settings
        * DSPlayer
          * Video Renderer: madVR  
            * Manage settings with Kodi: Load from madVR active profile
            * Direct3D presentation: Direct3D 11
          * Audio Renderer: Internal Audio Renderer (SaneAR)  
          * Filters management: Internal filters  
            * Video Decoder
              * Enable System Tray Icon: On  
              * Hardware decoder to use: D3D11  
            * Audio Decoder (OPTIONAL: for bitstreaming)
              * Enable System Tray Icon: On  
              * Bitstreaming \<codec\>: On  

* *Test*
  * *Kodi app*
    * Play a [test HDR video](/wiki/hdr#hdr-tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 33ms for 30fps, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  
* *Update MadVR* (OPTIONAL)
  * If you want newer, beta madVR features, after validating your setup, [download madVR beta](https://madshi.net/madVRhdrMeasure113.zip), unzip and copy the files into C:\Program Files (x86)\K-Lite Codec Pack\Filters\madVR\  

### **JRiver Media Center**

HDR passthrough or simple/dynamic tonemapping.  

[See here](https://www.avsforum.com/threads/valerion-visionmaster-pro-2-and-max-owners-thread.3314095/page-172?post_id=64069504#post-64069504)

### **Potplayer**

Simple, HDR passthrough or tonemapping.  

* *Requirements:*  
  * Common settings above  
  * Install [Potplayer](https://potplayer.daum.net/)  
* *Windows 1x settings:*  
  * Settings app -> System -> Display -> HDR and WCG/Use HDR/Play HDR.. -> **Off**  
* *Potplayer settings:*  
  * *Potplayer app*  
    * Preferences -> Video
      * Video Renderer: Built-in Direct3D 11 Video Renderer
      * Use H/W HDR Output Mode: ON *(OFF to tonemap to SDR)*
    * Preferences -> Video -> Pixel Shaders
      * Enable SMPTE ST 2084 HDR Correction: OFF *(ON to tonemap to SDR)*
      * Enable SMPTE ST 2086 HDR Correction: OFF *(ON to tonemap to SDR)*
    * *OPTIONAL*: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart Potplayer app*  
* *Test*  
  * *Potplayer app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

### **Plex HTPC**

Simple, HDR Passthrough or Tonemapping  

* *Requirements:*  
   * Common settings above  
   * Install Plex HTPC: Windows: >= 1.16: ([download](https://www.plex.tv/media-server-downloads/?cat=plex+htpc&plat=windows#plex-app)), Linux: >= 1.60.1: ([download](https://snapcraft.io/plex-htpc))  
   * *Notes:*  
     * If HDR is not configured as per below, HDR will be tonemapped to SDR. Available for Windows, Linux and Mac.  
* *Plex HTPC settings:*  
   * *Plex HTPC app*  
     * Settings -> Video
        * Enable HDR Switching: Checked  
        * HDR Metadata Passthrough: Checked  
* *MPV settings (Linux) **EXPERIMENTAL**:*  
   *  Create/Edit file: ~/snap/plex-htpc/common/mpv.conf
      * Add:  
     `[HDR]`<br>
     `profile-cond=p["video-params/primaries"] == "bt.2020"`<br>
     `vo=gpu-next`<br>
     `hwdec=auto-copy`<br>
     `target-colorspace-hint=yes`<br>
     `target-trc=pq`<br>
     `target-prim=dci-p3`<br>
     `dolbyvision=no`<br>
     <!--
     MISC
     `target-contrast=inf ##inf is for OLED, for LCD get the contrast value from rtings or similar`<br>
     `target-peak=700    ## If you have an HDR display, adjust this to the 10% peak`<br>
     HDR->SDR TONEMAPPING
     `target-colorspace-hint=no`<br>
     `gamut-mapping-mode=clip`<br>
     `vf=format:dolbyvision=no:hdr10plus=no`<br>
     `tone-mapping=st2094-10`<br>
     `target-peak=100`<br>
     `hdr-compute-peak=yes`<br>
     `allow-delayed-peak-detect=yes`<br>
     `hdr-peak-percentile=99.9`<br>
     `target-prim=bt.2020`<br>
     `target-trc=pq`<br>
     `saturation=-20`<br>
     MESA 25.1+ HDR
     `vo=gpu-next`<br>
     `hwdec=vulkan`<br>
     `gpu-api=vulkan`<br>
     `gpu-context=waylandvk`<br>
     `target-colorspace-hint=yes`<br>
     `target-trc=pq`<br>
     -->
* *Test*
  * *Plex HTPC app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  

&nbsp;

### **MPV (Linux) EXPERIMENTAL/DRAFT**

Simple, HDR Passthrough or Tonemapping  

* *Requirements:*  
   * Common settings above (Linux Desktop)
   * Enable OS HDR
     * System Settings->Display Configuration->Enable HDR: Checked, Color accuracy: Prefer color accuracy, Calibrate HDR brightness
   * Install MPV: Terminal->`sudo snap install mpv`
   * *Notes:*  
     * If HDR is not configured as per below, HDR will be tonemapped to SDR (?)
* *MPV settings:*  
   *  Create/Edit file: ~/snap/mpv/current/.config/mpv/mpv.conf
      * Add:  
     `[HDR]`<br>
     `profile-cond=p["video-params/primaries"] == "bt.2020"`<br>
     `vo=gpu-next`<br>
     `hwdec=auto-copy`<br>
     `target-colorspace-hint=yes`<br>
     `target-trc=pq`<br>
     `target-prim=dci-p3`<br>
     `dolbyvision=no`<br>
     <!--
     MISC
     `target-contrast=inf ##inf is for OLED, for LCD get the contrast value from rtings or similar`<br>
     `target-peak=700    ## If you have an HDR display, adjust this to the 10% peak`<br>
     HDR->SDR TONEMAPPING
     `target-colorspace-hint=no`<br>
     `gamut-mapping-mode=clip`<br>
     `vf=format:dolbyvision=no:hdr10plus=no`<br>
     `tone-mapping=st2094-10`<br>
     `target-peak=100`<br>
     `hdr-compute-peak=yes`<br>
     `allow-delayed-peak-detect=yes`<br>
     `hdr-peak-percentile=99.9`<br>
     `target-prim=bt.2020`<br>
     `target-trc=pq`<br>
     `saturation=-20`<br>
     MESA 25.1+ HDR
     `vo=gpu-next`<br>
     `hwdec=vulkan`<br>
     `gpu-api=vulkan`<br>
     `gpu-context=waylandvk`<br>
     `target-colorspace-hint=yes`<br>
     `target-trc=pq`<br>
     -->
* *Test*
  * *MPV app*  
    * Play a [test HDR video](/wiki/hdr#hdr-tests). [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.
    * ALT: `ENABLE_HDR_WSI=1 mpv --gpu-api=vulkan --gpu-context=waylandvk "/path/to/video_file"`  

&nbsp;

### **Plex Media Player (old)**

Simple, Tonemapping  

* *Requirements:*
  * Common settings above
  * Plex Media Player 2.x
  * *Notes:*
    * HDR is not currently passed through; It is tonemapped to SDR. Available for Windows, Linux and Mac.  
* *Plex Media Player settings:*  
  * None  

## Streaming Content (Netflix, Youtube, etc..)

* *Requirements:*
  * Common settings above
  * Netflix: ALL displays have HDCP 2.2 support and are recognized. Check Nvidia/AMD/Intel graphics control panel for HDCP status. Required software is installed: Microsoft Store [HEVC Extension](https://www.microsoft.com/en-us/p/hevc-video-extensions/9nmzlz57r3t7), Intel MEI driver/ME firmware (Intel iGPU). Required [Premium Plan](https://help.netflix.com/en/node/24926) subscription. 
  * Supported Web Browsers/Apps: Microsoft Edge (Netflix/Youtube), Microsoft Store app (Netflix), Google Chrome (Youtube)  
* *Windows settings:*  
  * Activate HDR
    * HDR may need to be turned on manually before viewing content; apps may not switch to HDR mode automatically like some local players do, especially in non-fullscreen mode. If that's the case, you can use the "Win + Alt + B" shortcut to turn on/off HDR in windows or the [HDRTray](https://github.com/res2k/HDRTray) utility to enable it via a mouse in the system tray.  
      * Start -> Settings -> System -> Display
        * Windows 10
          * Windows HD Color settings
            * Use HDR: On / Play HDR games and apps: On (Wording depends on Windows version)  
            * Stream HDR Video: On  
        * Windows 11
          * HDR
            * (Use) HDR: Off  
              * Allow HDR video streaming even when HDR is off: On  
            * HDR video streaming..: On  
* *Test*
  * Netflix: Check edge://gpu in Microsoft Edge for: HDCP 2.2 support, HEVC installed/activable, and HEVC - HDR10 support set true. Check [Netflix HDR10 test pattern](https://www.netflix.com/title/80018499) looks correct.
  * Youtube: <!-- Check edge://flags in Microsoft Edge for: Media Foundation for Clear set to Enabled. --> Check [HDR content](https://www.youtube.com/watch?v=njX2bu-_Vw4) looks correct.

## HDR Tests

[Our HDR10 Test Videos/Patterns](https://drive.google.com/uc?export=download&id=1HbVqzhhtncjkowdxBgZ-ghycvy5w2cpv) - For Basic HDR video calibration  
[Mehanik's Full HDR10 Test Videos/Patterns](https://drive.google.com/drive/folders/1m4IBq0euAxamL9ePgfdFuf8_5nLcRwHA) - For Advanced HDR video calibration  
[Ideal 4K HEVC HDR10 test](https://drive.google.com/uc?export=download&id=1Q2Ix3mXMl-EMs0-hE-C3gCHg_Uwh4HZz) - UHD Blu-Ray high bitrate test - 4k, HEVC, HDR10, 50-90Mbps, 10-bit, 29.97fps, mp4  
[Dolby's HDR tests](https://ott.dolby.com/browser_test_kit/help_files/topics/r_test_signals_all.html#r_files_mp4_all_def) - Multiple resolutions, frame rates and HDR types - 480p->4k, HEVC, HDR10/HLG/DV, DD+Atmos, mp4  

## Appendix

### MadVR Performance Settings Per GPU

WARNING: These settings are for more intensive image processing/scaling of <= 1080p to 4k, that is **NOT** necessary for just HDR passthrough.  
They are not the end all to be all and are best when configured with [resolution-conditional profiles](https://yabb.jriver.com/interact/index.php?topic=124136.0) to limit upscaling on higher resolutions, like 4K, which are beyond the scope of this page.  
The settings below are also **conservative** so you don't have to spend hours wasting your time with stuttering due to high rendering times and diminishing returns. **Test with the default settings above before changing to any of these**. Don't test higher tiers until you test the conservative ones first.  
This doesn't mean that they're not gpu intensive; they most certainly are.  
If you can't handle the GPU load/noise/heat these settings produce, turn them down or go back to the madvr Bilinear defaults.   
Related: [What are the best ways for scaling video?](/wiki/video#what-are-the-best-ways-for-scaling-video), [madVR beginner scaling](https://yabb.jriver.com/interact/index.php?topic=124136.0), [madVR settings](https://forum.doom9.org/showthread.php?p=1709584)  

GPU|IMAGE UPSCALING|IMAGE DOUBLING|IMAGE DOWNSCALING|CHROMA UPSCALING|DITHERING
:--|:--|:--|:--|:--|:--
Intel UHD >= 6xx|DXVA2|NA|DXVA2|BiCubic 75+AR|random
AMD Ryzen Vega xx|Cubic/Lanczos|NA|Cubic/Lanczos|BiCubic 75+AR|random
Nvidia GT 1030/Ryzen RDNA 6xxM/740M|Lanczos 3-tap+AR|NA|Lanczos 3-tap+AR|BiCubic 75+AR|random
Nvidia GTX 960/1050/1050 Ti/Ryzen RDNA 760-780M|Lanczos 4-tap+AR|NA|SSIM 1D+LL+AR|Jinc+AR|random
Nvidia GTX 1650|Lanczos 4-tap+AR|NGU Standard Luma Low|SSIM 1D+LL+AR|NGU Standard Low|random
Nvidia GTX 1650 Super|Lanczos 4-tap+AR|NGU Standard Luma Low|SSIM 1D+LL+AR|NGU Standard Low|Error Diff. #1
AMD RX 5xx|Jinc|NGU Standard Luma Low (Med: 570/580)|SSIM 1D+LL+AR|super-xbr 100+AR|Error Diff. #2
Nvidia GTX 970/1060|Jinc|NGU Standard Luma Med|SSIM 1D+LL+AR|NGU Standard Low|Error Diff. #1
Nvidia GTX 980/1660 (Reg/Ti/Super)/3050 6GB|Jinc|NGU Standard Luma High|SSIM 1D+LL+AR|NGU Standard Med|Error Diff. #2
Nvidia GTX >= 1070/RTX 2060/3050 8GB|Jinc|NGU Sharp Luma High|SSIM 1D+LL+AR|NGU Standard Med|Error Diff. #2
AMD RX 56xx - 66xx|Jinc|NGU Standard Luma High|SSIM 1D+LL+AR|NGU Standard Med|Error Diff. #2
AMD RX >= 67xx|Jinc|NGU Sharp Luma High|SSIM 1D+LL+AR|NGU Standard Med|Error Diff. #2

### Alternate MPC-HC/MPC-BE + madVR Install Method

* *Requirements:*  
  * MPC-HC/MPC-BE: 
    * MPC-HC: Install MPC-HC from exe ([download](https://github.com/clsid2/mpc-hc/releases))
    * MPC-BE: Install MPC-BE from installer: ([download](https://github.com/Aleksoid1978/MPC-BE/releases))
  * MadVR: Install madVR from stable zip ([download](http://madshi.net/madVR.zip))
    * Extract/copy madVR directory in zip to directory: %USERPROFILE%\
    * Go into extracted directory %USERPROFILE%\madVR, right-click on 'install.bat' script and click on Run as administrator option to install.
* *madVR settings:*  
  * Run %USERPROFILE%\madVR\madHcCtrl.exe program. Double-click on the 'mad* home cinema control' icon in your system tray
    * devices
      * \<your_display_device\>
        * properties -> PC levels 0-255, bitdepth: 10 bit or higher  
        * calibration -> this display is already calibrated  
        * display modes (OPTIONAL - for refresh rate switching)
          * Enable: switch to matching display mode..when playback starts  
          * list all display modes..: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60 (assumes a 4k display)  
        * HDR -> passthrough HDR content to the display, send HDR metadata to the display  
          * *ALT: For static tonemapping to SDR*: HDR -> let madVR decide + rendering->trade quality for..->don't measure HDR.. option checked
    * scaling algorithms
      * chroma upscaling
        * processing..: Bilinear (for more intensive scaling, see Performance settings section at the bottom)  
      * image downscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
      * image upscaling
        * processing..: Bilinear/DXVA2 (for more intensive scaling, see Performance settings section at the bottom)  
    * rendering
      * general settings
        * Enable: delay playback start.., enable automatic fullscreen exclusive mode, use Direct3D 11 for presentation  
        * **If** frame drops/stuttering occur while testing, increase CPU/GPU queue size here
      * dithering
        * algorithm: Ordered dithering (unless you have dedicated GPU, see settings section below)  
  * Apply -> Ok. Right-click -> Exit the 'mad* home cinema control' icon in your system tray
* *MPC-HC/BE settings:*  
  * *MPC-HC app*  
    * View -> Options
      * Playback -> Output
        * DirectShow Video: madVR  
      * Internal Filters -> Video Decoder  
        * Hardware Decoder to use: 'D3D11' (win 8/10/11) or DXVA2 (copy-back) (win 7) 
        * Hardware Device to use: \<your_GPU_device\> 
        * RGB output levels: PC (0-255) (see VIDEO setup guide if not sure) 
      * *OPTIONAL*: Audio: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart MPC-HC app*  
  * *MPC-BE app*  
    * View -> Options
      * Video
        * Video Renderer: madVR  
      * Internal Filters -> Video Decoders  
        * Video decoder configuration  
          * Preferred Decoder: 'D3D11, DXVA2' (win 8/10/11) or DXVA2 (win 7) 
          * Adapter: \<your_GPU_device\> 
          * RGB output levels: PC (0-255) (see VIDEO setup guide if not sure) 
      * *OPTIONAL*: Audio: [Wiki:Audio Setup Guide](https://r-htpc.github.io/wiki/audio#softwareos-setup)
    * *Restart MPC-BE app*  
* *Test*  
  * *MPC-HC/BE app*  
    *  Play a [test HDR video](/wiki/hdr#hdr-tests) and press Ctrl+J to show stats. If avg/max rendering stats are >= 33ms for 30fps, you're either doing too much madVR processing or your GPU isn't powerful enough. [If the colors in your video are washed out](https://i.imgur.com/AD6lOIS.jpg), either you don't have proper hardware support for HDR, aren't using HDMI 2.x ports, or don't have TV deep color configured.  
* *Update MadVR* (OPTIONAL)  
  * If you want newer, beta madVR features, after validating your setup, [download madVR beta](https://madshi.net/madVRhdrMeasure113.zip), unzip/copy all the FILES (NOT the directory itself) inside the zip into your previously-created %USERPROFILE%\madVR directory

### Fullscreen Exclusive (FSE) behavior not working
* *Disable fullscreen optimizations*: Find your video app/player's .exe file, right-click->Properties->Compatability->Disable fullscreen optimizations: enabled->Ok. Reboot  
* *Disable Game DVR (registry)*: Download and run this [reg file](https://gist.github.com/Redrrx/a6680e0b9fd0a1386efa3cf736ecde2e). Reboot
* *Disable Game Bar/DVR (app)*: In Windows 11 settings app under Gaming

<!-- Footer -->
&nbsp;

---

*This page was last updated on 2025-12-19*

