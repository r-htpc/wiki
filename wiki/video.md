# Video Setup Guide

*This page is best viewed with a PC web browser.*  

**THIS PAGE IS IN A DRAFT STATE AND UNDER CONSTRUCTION**

<!-- Section -->

## How do I configure my htpc/media device for video?

Please read the Video Formats and Transports sections before you embark on the sections below it, so you understand the terms and concepts mentioned.  

For simplicity, the term "HTPC" here can mean either a PC or a streaming device, like a Roku/Fire TV/etc, except where differences are noted.  

<!-- Sub-Section -->

### **Video Formats/Codecs**

x264: Also known as h.264/MPEG-4 AVC. A very common lossy video compression codec. Used in Netflix, newer HD blu-ray discs and ATSC 1.0 OTA. Optimal for resolutions <= 1080p.  
x265: Also known as h.265/MPEG-H HEVC. The successor to AVC with better, but still lossy, compression. Used in 4k Netflix, UHD blu-ray discs and ATSC 3.0 OTA. Optimal for resolutions >= 1440p.  
Xvid/Divx: Also known as h.263/MPEG-4 Part 2. Xvid is an open-source version. An old compression codec commonly used in AVI and Divx containers.  
VC-1: Used in newer HD blu-ray discs  
VP9: A compression codec used on Youtube  
AV1: A modern, lossy compression codec currently with limited support. The successor to HEVC and VP9  
MPEG-2: Also known as h.262/MPEG-2 Part 2. A low compression codec. Used in DVDs, old HD blu-ray discs and ATSC 1.0 OTA. Commonly used with the TS container

<!-- Sub-Section -->

### **Video Containers**

MP4: Modern video container supporting a single video/audio/subtitle stream. Commonly used with the AVC/h264 video codec and AAC audio codec.  
MKV: A modern video container supporting multiple video/audio/subtitle streams. Menu/chapter support.  
AVI: An old video container supporting a single video/audio stream. No subtitle stream support. Usually used with Xvid/Divx codec.  
DIVX: An old video container extension of AVI. Used on some old DVDs. Usually used with Xvid/Divx codec.  
VOB: A video container for DVDs using MPEG-2 or MPEG-1.  
TS: Also known as MPEG-TS. Used with MPEG-2 codec for tv broadcasts.  
M2TS: An extension of MPEG-TS. Used with old HD blu-ray discs and MPEG-2.  
BDMV/BDAV: Used in HD/UHD blu-ray discs. BDMV has menu capability, BDAV does not and is a modified MPEG-2 TS container using x264, MPEG-2 or VC-1.  

<!-- Sub-Section -->

### **Video bitrates**

An aggregation of video content information encoded in a pixel over time. Usually referenced in Mbps.  
A lower bitrate indicates less video information which can induce video artifacting, blurring, and color banding  
A decent bitrate for 1080p AVC/x264 content is 5 Mbps. A high bitrate is 25 Mbps.  
A decent bitrate for 4K HEVC/x265 content is 20 Mbps. A high bitrate is 100 Mbps.  
It is recommended to aim for at least 0.1 bits per pixel (BPP) when encoding video content. Video with lots of motion or scenes that are prone to color banding (sky, under-water) will require higher BPP.  
You can calculate video bitrate by applying the formula  
 Resolution width * Resolution height * fps * bpp / 1000000 = Mbps  
 e.g. 1920 * 1080 * 23.976 * 0.1 / 1000000 = 5 Mbps  

<!-- Sub-Section -->

### **Video Transports/Interfaces**

HDMI 1.4: Digital. 10 Gbps. 4K @ 30 Hz  
HDMI 2.0: Digital. 18 Gbps. 4K @ 60 Hz. HDR  
HDMI 2.1: Digital. 48 Gbps. 4K @ 120 Hz. HDR+  
Displayport 1.2 (native): Digital. Displayport on both ends. 20 Gbps. 4K @ 60 Hz  
Displayport 1.4 (native): Digital. Displayport on both ends. 32 Gbps. 4K @ 120 Hz. HDR  
Displayport (Alternate mode): Digital. Displayport/USB->HDMI cable/adapter  

<!-- Sub-Section -->

### **Video Metadata/Color Technologies**

**HDR Types**

HDR10: Very common. Very compatible. Static Metadata. 400-4000 cd/m2. 10-bit color.  
HDR10+: Not common. Dynamic Metadata. 1000-4000 cd/m2. 10-bit color.  
Dolby Vision: Very common. Not very compatible, esp. with local content. Dynamic Metadata. 1000-4000 cd/m2. 12-bit color.  
HLG: Not common. No metadata. SDR & HDR in same signal. 1000 cd/m2 nominal. 10-bit color.  

**Color Technologies**

1. Color Primaries:  
 a. Rec 709 (1080p/4k 8/10-bit SDR)  
 b. sRGB (8-bit SDR, Windows default)  
 c. P3 (8/10-bit SDR/HDR)  
 d. Rec 2020 (4k/8k 10/12-bit SDR/HDR)  
 e. Rec 2100 (1080p/4k/8k 10/12-bit HDR)  
2. Transfer Functions: Gamma (Rec 709, sRGB), PQ (Rec 2020, Rec 2100), HLG (HLG)  
3. Formats: ST 2084 (Optional static metadata), ST 2086 (Static metadata), ST 2094 (Dynamic Metadata)  
4. Technology Combinations (TECHNOLOGY: BIT-DEPTH, TRANSFER FUNCTION, COLOR PRIMARIES, FORMATS)  
 a. PQ10: 10-bit, PQ, P3->Rec.2020, ST 2084  
 b. HDR10: 10-bit, PQ, P3->Rec.2020, ST 2084/ST 2086  
 c. HDR10+: 10/12-bit, PQ, P3->Rec.2020, ST 2094  
 d. Dolby Vision: 10/12-bit, PQ, P3->Rec.2020, ST 2094  
 e. HLG: 10-bit, HLG/Gamma, P3->Rec.2020, None    
 f. DVD/FHD Blu-Ray: 8-bit, Gamma, Rec.709->sRGB, None  
 g. UHD Blu-Ray: 10/12-bit, PQ, P3->Rec.2020, ST 2084/ST 2086/ST 2094  
 h. Online Streaming: 8/10/12-bit, Gamma->PQ, Rec.709->Rec.2020, None/ST 2084/ST 2086/ST 2094  

<!-- Sub-Section -->

### **Video Hardware**

1. GPU
 - iGPU: A graphics card built into the CPU  
 - dGPU: A graphics card separate from the CPU. Usually found on a PCIe expansion card.  
 - eGPU: A graphics card external to the HTPC, connected to it via USB/Thunderbolt.  
2. Display
 - TV  
 - Projector  

<!-- Sub-Section -->

### **Video Software**

See also: [Audio Software](/htpc-wiki/audio#audio-software)  

**Media Servers**

1. [Plex](https://plex.tv) - Media server software that streams content out to clients. Distinguishing features include:  
 -  Support for Windows, Linux, Mac  
 -  Support for live tv via tv tuners  
 -  Automatic scanning of video content directories  
 -  Automatic retrieval of metadata content (posters, descriptions, trailers) from the internet  
 -  Real-time transcoding video/audio down to other containers, codecs, resolutions and bitrates via CPU/GPU  
 -  Streaming of video content to remote video clients  
 -  Support for playback via windows, linux and web browser clients  
 -  Intro skip, Credit skip, Media collections, Subtitle support  
 -  HDR tonemapping support  
2. [Emby](https://emby.media)  
3. [Jellyfin](https://jellyfin.org)  

**Players**

1. [Kodi](https://kodi.tv) - An open source media player/center.  
 - Support for Windows, Linux, Mac, Android  
 - Automatic scanning of video content directories  
 - Automatic retrieval of metadata content (posters, descriptions) from the internet  
 - Extensive plug-in support  
 - [HDR support](/htpc-wiki/hdr), Subtitle support  
 - MadVR integration  
2. [Plex](https://plex.tv) - A media player that interfaces with the Plex Media Server and plex.tv video content  
 - Support for Windows, Linux, Mac, Android  
 - [HDR support](/htpc-wiki/hdr), Subtitle support  
3. [VLC](https://www.videolan.org/vlc/)  
 - Support for Windows, Linux, Mac, Android  
 - [HDR support](/htpc-wiki/hdr)  
 - DVD/Blu-ray folder support  
4. PotPlayer  
 - MadVR integration  
 - HDR support (via MadVR)  
 - Not open source
5. [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases)/[MPC-HC](https://github.com/clsid2/mpc-hc/releases/)  
 - Support for Windows  
 - Extensive feature-set
 - MadVR integration  
 - [HDR support (via MPC VR/MadVR)](/htpc-wiki/hdr)  
 - Subtitle support  
 - DVD/Blu-ray folder support  
6. [JRiver Media Center](https://jriver.com/)  
 - Support for Windows, Mac, Linux  
 - Automatic scanning of video content directories  
 - Automatic retrieval of metadata content (posters, descriptions) from the internet  
 - MadVR integration  
 - HDR support  
 - Commercial
7. [MPV](https://mpv.io)  
 - Support for Windows, Linux, Mac, Android  
 - Minimal GUI  
 - HDR support  
8. PowerDVD  
 - DVD/Blu-ray/UHD Blu-ray disc support  

**3rd Party**

1. [MediaInfo](https://mediaarea.net/en/MediaInfo) - Extremely useful tool for getting various video & audio information (codecs, formats, etc..) on media files  
2. [MPC VR](https://github.com/Aleksoid1978/VideoRenderer) - Simple video renderer used to enable HDR passthrough, HDR tonemapping, Resolution/Chroma upscaling, Dithering  
3. MadVR - Advanced video renderer used to enable HDR passthrough, HDR tonemapping, Resolution/Chroma upscaling, Dithering, Resolution/Refresh Rate Switching  
4. SVP - Used to upscale frate-rates for video smoothing  
5. [K-lite](https://codecguide.com/download_kl.htm) - Codec pack including various video software  
 - Video/audio codecs  
 - Video/audio filters/splitters/mixers  
 - MPC VR, MadVR  
6. LAV Filters - ffmpeg based DirectShow media software including:  
  - Splitters, Decoders, Filters, Mixers and Compressors  
  - Automatic stream selection  
7. Virtual CloneDrive 
  - Mount ISO files for disc playback support  

<!-- Section -->

## Setup

**Hardware Setup**  

See the [AUDIO Setup Guide](/htpc-wiki/audio#setup) for different ways of connecting your HTPC to a display and sound system.  

**Software/OS Setup**  

Make sure the video driver for your GPU is installed, updated from the GPU vendor, and working.  

Set up your app/gpu driver/tv settings for color reproduction. See [section below](/htpc-wiki/video#setup-for-color-reproduction).  

Run video calibration tests to make sure the above setup is correct. See [section below](/htpc-wiki/video#video-calibration-testing).  

Run motion calibration tests for judder/stutter. See [section below](/htpc-wiki/video#motion-calibration-testing).  

Configure your video player application for hardware decoding. See [section below](/htpc-wiki/video#application-specific-setup-for-hardware-decoding).  

OPTIONAL: Application-Specific Setup For Resolution/Refresh Rate Switching. See [section below](/htpc-wiki/video#application-specific-setup-for-resolutionrefresh-rate-switching).  

OPTIONAL: Application-Specific Setup For HDR/Scaling. See [section below](/htpc-wiki/video#application-specific-setup-for-hdrscaling).  

<!-- Sub-Section -->

### **Setup For Color Reproduction**

While researching setup of your devices you may have come across confusing terms like YCbCr, RGB, RGB full/limited, black level.  

First, let's get YCbCr and RGB out of the way. These are color spaces for encoding content. RGB treats blacks, whites and colors equally. YCbCr treats blacks and whites differently than colors, in that it compresses colors such that our eyes can't really tell the difference between it and RGB; this saves bandwidth.  
YCbCr is common for video content. RGB is common for games and the desktop.  

Now, to RGB full/limited. In short, RGB full/limited is just different numbering systems to apply to the range of white to black.  

RGB Full denotes 0 as Black and 255 as White. RGB Limited denotes 16 and below as Black and 235 and above as White.  

What makes this confusing is a setting of Full or Limited can be on multiple pieces of your system, more specifically:  

1. The Application (The video renderer (madVR/MPC VR/EVR CP) in what you're using to play/decode/render your content, Kodi, Plex, MPC, etc..)  
2. The GPU driver (nvidia, amd, intel, etc..)  
3. The Display (TV, Projector)  

If you set each piece in the wrong combination, whites and blacks will look wrong, colors will be washed out and/or shadows/details will be diminished.  
Without getting too into the weeds, here's what you should set for the 3 pieces above, depending on your scenario, but use #1 first, where at all possible.  

Scenario #1 - PC Recommended:  
 - Display: Color Space: RGB, Range: Full.  
 - GPU: Color Space: RGB 8-bit, Range: Full  
 - Application: Range: Full (0-255), Bit depth: auto/<display bit depth>  
Scenario #2 - PC Alternate:  
 - Display: Color Space: RGB, Range: Limited  
 - GPU: Color Space: RGB 8-bit, Range: Full  
 - Application: Range: Limited (16-235), Bit depth: auto/<display bit depth>  
Scenario #3 - Media device (roku, shield, fire tv) video content on a TV:  
 - Display: Limited  
 - GPU: Color Space: YCbCr/YUV 422 12-bit  
 - Application: Limited (16-235), where available  

To confuse things even more, sometimes Full and Limited are called by other names. We urge you to read a primer on calibration settings which explains more of the terms you'll find in your Display and what they're called for each major mfgr. The page at [rtings.com](https://www.rtings.com/tv/learn/how-to-calibrate-your-tv) is a good one to start with. If you still can't figure out what ranges are available on your Display, **assume it's in Limited range by default** unless you change it (like put in PC mode) or your manual says otherwise.  

**After all that, make the changes based on the above 3 scenarios. As mentioned above, when in doubt, use #1, as exampled with the following for a PC**

1. Change the color space on your Display to RGB/Native (where available) or Auto. Change the input range to Full. As a last resort, put your Display in PC or Game Mode. This will remove a lot of Display processing options, so if this is not desired, you may want to use Scenario #2's Limited settings for this step and step #3.  
2. Change your GPU driver settings to a color space of RGB, a color depth of 8-bit, a resolution of what you want (1080p/2160p), and a refresh rate of 60 Hz (or 120 hz where available)  
3. Change your video application's renderer to a Range of Full (0-255). This is the default for all renderers (madVR/MPC VR/EVR CP) unless otherwise changed. Change Bit depth to auto  

<!-- Sub-Section -->

### **Video Calibration Testing**

We know it is tempting to install and configure every software you want to use right away and get on to playing content; but doing everything all at once usually leads to problems which become hard to diagnose once you've added so much software and configuration layers on top of your base OS.  
As such, it is highly recommended to run video calibration tests before you play content so you know you've set up the combination of your app/gpu/display properly to get the proper colors, whites/blacks, and motion for the media content you will be playing.  

To do this, you should
 
1. Set the proper color conversion/reproduction settings [from above](/htpc-wiki/video#setup-for-color-conversion-reproduction).  
2. Calibrate your display in Windows. Start->Color Management->Advanced->Calibrate Display  
3. **Disable** Hardware Decoding/Acceleration (DXVA, D3D11, NVDEC, pixel shaders etc..) in your video player application, where at all possible, to minimize the chance of the GPU decoder/renderer messing up colors, blacks and whites. You can re-enable it after you're done. The language is different depending on your media player. It should be set to Software/None/Acceleration disabled/etc.. as per the option locations in the below Decoding section.      
4. Download calibration media like [AVS HD 709](https://www.avsforum.com/threads/avs-hd-709-blu-ray-mp4-calibration.948496/). Get the MP4 version. At the minimum, extract the tests from the 'Basic Settings' and 'Misc Patterns->A' folder.  
5. Read the [AVS manual](https://www.w6rz.net/avshd709/Patterns-Manual.pdf) and then run the calibration tests in your video player application.  
6. If everything looks good, enable Hardware Decoding/Acceleration in your media player as per the below section. If everything does NOT look good, you messed something up in #1/#2. Go back and re-check/re-try.  
7. Re-run the AVS calibration tests.  
8. If everything in the tests look good, start playing some test content. Start with known-good content, like the jellyfish and non-HDR real-world [files below](/htpc-wiki/video/#where-do-i-find-additional-sample-video-files-to-test). Work your way up from lower resolutions and common codecs (h264) to the resolutions, codecs, and formats you want to use. For example, start with 1080p:h264:8-bit:SDR, then 1080p:HEVC:10-bit:SDR, then 4k:HEVC:8-bit:SDR. This tiered approach will help you find any potential problems along the way. If you're dropping frames from the content, experiencing stutter or judder, consult the appropriate sections below.  
9. If everything in the tests look good, make any additional video setting changes you desire ([enabling HDR, changing renderers, upscaling](/htpc-wiki/hdr), etc..) and play the test content again. If you've enabled HDR, use the HDR test videos/patterns and the real-world files below for that.  
10. If everything in the tests does NOT look good, either there's something messed up in your GPU color conversion/decoding, your display device is limiting you (e.g. HDR luminance/tonemapping), or your GPU/renderer is limiting you (e.g. aggressive post-processing). Check settings from #8, re-test, and/or seek help on the sub.  
11. Move on to Motion Calibration Testing or start playing real content.  

<!-- Sub-Section -->

### **Motion Calibration Testing**  

This section is UNDER CONSTRUCTION.  

You will first run a test for the presence of motion problems like stutter. You will do this under a no-judder condition where the content frame rate and display refresh rate match. After that you will test for judder itself and how bad it is for you subjectively.  

1. Set your display (through the GPU driver) to a specific refresh rate equal to the content you want to test. e.g. 24Hz for 24fps content.
2. Test that the refresh rate is set correctly and consistently using [this test](https://www.testufo.com/refreshrate).  
3. Test playing content and look for any observable motion problems. Here is test [24p content](https://www.youtube.com/watch?v=oy8wNzOGVmc)/[25p content](https://www.youtube.com/watch?v=Ou3QXsTro7A)/[60p content](https://www.youtube.com/watch?v=RgGwWN9EC8g).
4. If you see a motion problem, **it's not judder**, and likely some form of stuttering. You should solve this problem before you move on. See the section "Why is my video playback stuttering and/or dropping frames?" below and repeat the tests.  
5. If you don't see a motion problem, and you plan to play content on a refresh rate that's not a multiple of your content frame rate (e.g 24p/25p on 60 Hz, 24p on 25Hz/50Hz), you should continue on to test for judder.  
6. Set your display (through the GPU driver) to the desired non-multiple refresh rate. e.g. 60 Hz for 24 fps content.  
7. Test that the refresh rate is set correctly and consistently using [this test](https://www.testufo.com/refreshrate).  
8. Test playing content and look for any observable judder. Here is test [24p content](https://www.youtube.com/watch?v=oy8wNzOGVmc)/[25p content](https://www.youtube.com/watch?v=Ou3QXsTro7A).  
9. Judder will likely be present; what's important is how bad it is and if it's something that's too distracting that you can't ignore. If you can't ignore it, see the section "How do I fix judder on my htpc?" below and repeat the tests.  

<!-- Sub-Section -->

### **Application-Specific Setup For Hardware Decoding**

Most video players have hardware decoding support built-in.  

Configuration usually involves a single toggle on the simple side, or, on the advanced side, choosing between DVXA/D3D11/Quicksync and/or choosing your proper GPU Device. Make sure your GPU Device supports hardware decoding for the format(s) you're trying to play. See the [GPU Feature Set Matrix](/htpc-wiki/faq/#graphics-gpus) of the FAQ.  

If configured correctly, CPU Usage should be low during playback, while GPU Usage (Decode/3D) should be higher in proportion. If GPU Decode/3D is 0, then hardware decoding is not being used.

MPC-BE:  
1. View->Options->Internal Filters->Video Decoders->Video Decoder Configuration: Codecs: <all checked>, Preferred Decoder: D3D11 (Win 8+) or DXVA2 (copy-back) (others)

MPC-HC:  
1. View->Options->Internal Filters->Video Decoder: Hardware Decoder to use: D3D11 (Win 8+) or DXVA2 (copy-back) (others)  
2. View->Options->Internal Filters->Video Decoder: Hardware Device to use: Automatic (if D3D11) or Your_GPU_Device (DXVA2)

VLC:  
1. Tools->Preferences->Input/Codecs->Hardware accelerated decoding: D3D11 (Win 8+) or DirectX (others)

Plex:  
*- Plex HTPC/Play Media Player*  
1. Settings->Video->(Use) Hardware Decoding: Enable  
*- Plex for Windows*  
1. Settings->Player->Use Hardware Decoding: Enable  

Kodi:  
1. Settings->Player->Change to "Advanced" config view  
2. Settings->Player->Videos->Render Method: DXVA/Automatic  
3. Settings->Player->Videos->Allow hardware acceleration - DXVA2: Enable  
4. Press 'O' during playback to test for (HW) video decoder  
  
Potplayer: TODO  

<!-- Sub-Section -->

### **Application-Specific Setup For Resolution/Refresh Rate Switching**

If the media you're watching does not have a framerate that's a multiple of your refresh rate (e.g. 24p on 60 Hz) you may want your media player to switch your display into the proper refresh rate to eliminate judder and proper resolution to allow your TV to do upscaling. 

1. Kodi  

   *Kodi app ->*  

   -- Settings -> Player -> Videos  

    ---- Set Settings level to Expert

    ---- Adjust display refresh rate: On start/stop  
    ---- Sync playback to display: OFF

   -- Settings -> System -> Display

   ---- Allow 3:2 pulldown refresh rates: OFF  
   ---- Allow double refresh rates: ON  
   ---- Whitelist:  

    *If you have a 120 Hz GPU & display you can skip 24 Hz and 60 Hz*  
    ---- 2160p display: 3840x2160 23.98 Hz, 3840x2160 24 Hz, 3840x2160 50 Hz, 3840x2160 59.94 Hz, 3840x2160 60 Hz  
    ---- 1080p display: 1920x1080 23.98 Hz, 1920x1080 24 Hz, 1920x1080 50 Hz, 1920x1080 59.94 Hz, 1920x1080 60 Hz  

2. MPC-BE w/MPC Video Renderer  
    
   *MPC-BE app ->*  

   -- View->Options->Video->Fullscreen

   ---- Use autochange fullscreen monitor mode: ON

   *If you have a 120 Hz GPU & display you can set [ 120 ] for 02, 04, 05, 08*  
   ------ 01: [ 23 ] @ <your res>  
   ------ 02: [ 24 ] @ <your res>  
   ------ 03: [ 50 ] @ <your res>  
   ------ 04: [ 29 ] @ <your res>  
   ------ 05: [ 30 ] @ <your res>  
   ------ 06: [ 50 ] @ <your res>  
   ------ 07: [ 59 ] @ <your res>  
   ------ 08: [ 60 ] @ <your res>  

   ---- Change display mode before starting playback: ON  


3. MPC-HC/MPC-BE w/madVR  

   *We assume you've already installed madVR first. If not, see the instructions in the HDR Setup Guide instead*

   *madVR app ->*  

   -- Devices -> Your_Display_Device ->  

    ---- display modes -> switch to matching display mode..when playback starts  

    Enter all resolutions and refresh rates supported by your display that you want to switch to. *If you have a 120 Hz GPU & display you can skip p24 and p60*  
    ---- display modes -> list all display..:  
    ------ 2160p display: 2160p23, 2160p24, 2160p50, 2160p59, 2160p60  
    ------ 1080p display: 1080p23, 1080p24, 1080p50, 1080p59, 1080p60  

4. Plex. See [here](https://support.plex.tv/articles/htpc-settings/)  

<!-- Sub-Section -->

### **Application-Specific Setup For HDR/Scaling**

[HDR Setup Guide](/htpc-wiki/hdr)  

<!-- Section -->

## Common Questions

<!-- Sub-Section -->

### What are the best algorithms for scaling video?

Video scaling algorithms from Worst to Best (and generally least resource intensive to most) are:  

Nearest Neighbor, Bilinear, DXVA, Cubic (Mitchell Netravali), Cubic (BiCubic), Catmull-Rom, Lanczos 2/3, Spline, Jinc, SSIM (downscale), super-xbr, NGU Standard, NGU Sharp.  

The Anti-Ringing/AR option added on to any algo is ideal, where available.  

These are OBJECTIVE rankings, and not SUBJECTIVE. Visual preferences are subjective i.e. different for each person. Test the algos to find the sweet spot for your own visual and GPU load/noise preferences. Do not go past the [recommended algos for your particular GPU](/htpc-wiki/hdr#wiki_madvr_performance_settings_per_gpu) without extensive performance testing.  

Any algo beyond **Jinc** will produce diminishing returns compared to the amount of load and noise it subjects your GPU to and may be detrimental to your HT listening environment.  

MPC VR will allow you to go up to Jinc. madVR to NGU Sharp.  

<!-- Sub-Section -->

### Why is my video playback stuttering and/or dropping frames?

1. You haven't configured your video player to use your GPU to hardware decode video. See application-specific setup above.
2. Your GPU doesn't support hardware decoding for the video codecs you're trying to play and your CPU isn't powerful enough to software decode them. Determine what video codec you're attempting to decode (using something like [MediaInfo](https://mediaarea.net/en/MediaInfo)) and then see the GPU section of the wiki faq for what codecs are supported by your GPU. Buy a better [CPU](/htpc-wiki/faq#wiki_cpus.3A) or [GPU](/htpc-wiki/faq#wiki_gpus.2Fgraphics.3A).
3. You're running on the edge of what your CPU/GPU can do performance-wise for the video bitrates you're trying to play. The higher the video bitrate, the more stress put on your CPU/GPU. Set your video player's process priority to Above Normal. Play lower bitrate videos. Buy a better [CPU](/htpc-wiki/faq#wiki_cpus.3A) or [GPU](/htpc-wiki/faq#wiki_gpus.2Fgraphics.3A).
4. You're doing too much post-proccessing with your video renderer (MadVR, MPC, EVR, etc..). Do less post-processing - Lower/Disable upscaling/downscaling/dithering techniques (nearest-neighbor/bilinear).  Use a more efficient renderer. Buy a better [GPU](/htpc-wiki/faq#wiki_gpus.2Fgraphics.3A).
5. You're running your RAM in single-channel mode or haven't dedicated enough RAM to your iGPU. Run 2+ sticks of RAM in dual-channel mode for the best performance. If using an iGPU, dedicate as much RAM to it, in your BIOS, where possible.
6. Your CPU/GPU is doing too much work in the background. Audit windows Task Manager and disable background tasks and/or processes using the CPU/GPU (updates, antivirus, disk indexing).
7. Your video driver is out of date. Update it and/or re-install the driver clean after running [DDU](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html).
8. If you have an Nvidia GPU, in Nvidia Control Panel -> Manage 3D Settings, Set Vertical Sync: ON, Low Latency Mode:OFF, Power Management Mode: Prefer Maximum.
9. If you have an AMD GPU: In Radeon Settings, Display -> Radeon FreeSync: OFF, Graphics -> Enhanced Sync: OFF, Wait for Vertical Refresh: ON, either globally or create a app profile for your video player  
10. You've configured your windows power plan or video driver power settings to balanced/power saving. Test with your windows power plan set to High Performance. Test with your video driver power management set to maximum performance.
11. Your video player isn't good/good at playing the video codec(s) you're trying to play. Try a different one (MPC-BE, MPC-HC, Kodi, VLC, Jriver, MPV)
12. You're using an OLED TV, which can cause stutter due to the nature of the tech. Test with Motion Interpolation enabled on it. 

<!-- Sub-Section -->

### How do I fix judder on my htpc?

First, make sure what you're experiencing is actually judder and not stutter. Watch [this](https://www.youtube.com/watch?v=CuEZIJDEQyo&t=1s) video.  

If you do have judder, then do one or more of the following..  

1. Configure your video players to switch the video card refresh rate automatically to match the content being played. See [section above](/htpc-wiki/video#wiki_application-specific_setup_for_refresh_rate_switching)
2. Configure your video card settings to run at a refresh rate that matches the bulk of the content you play. PC: 23 Hz for 23.976 fps content.
3. If you can't/won't do #1 or #2. Set your refresh rate to a number that divides equally into the fps of the bulk of the content you play
. e.g. 120 Hz (for 24/30/60 fps). If you can't do this then set your TV to 60 Hz/120 Hz and configure judder reduction in your TV settings. Some TVs do this automatically. Others may call this "Cinema Screen", "Motion Flow/CineMotion" or "Film Mode"  
4. If you have an Nvidia GPU, in Nvidia Control Panel -> Manage 3D Settings, Set Vertical Sync: ON, Low Latency Mode:OFF, Power Management Mode: Prefer Max/Adaptive/Normal.
5. If you have an AMD GPU: In Radeon Settings, Display -> Radeon FreeSync: OFF, Graphics -> Enhanced Sync: OFF, Wait for Vertical Refresh: ON, either globally or create a app profile for your video player  
6. Use the [SVP (Smooth Video Project)](https://www.svp-team.com/) filter to up-convert the content's fps (e.g. 23.976 fps to 60 fps) before it gets to the display.  
7. Use a media device instead that can do automatic Refresh Rate Switching. Fire TV (Prime Video), Nvidia Shield (Netflix, Prime Video) (beta), Android TV+[SmartTubeNext](https://github.com/yuliskov/SmartTubeNext) (Youtube)  

<!-- Sub-Section -->

### What refresh rate should I run on my HTPC?

Whatever refresh rate matches the framerate of the bulk of the content you play, if automatic Refresh Rate Switching is not available.  
Content varies between 23.976, 24, 25 fps, 29.97 or 60 fps. Local content is usually 23.976 fps (23 Hz) in North America and 25 fps (25 Hz) in Europe. Youtube is 24/25/30/60 fps. Netflix is 23.976/24/25/29.97 fps.  

<!-- Sub-Section -->

### What is the best way to change DisplayPort/USB-C to HDMI. What are the limitations associated with doing this?

There are 2 ways to change DisplayPort to HDMI. The 1st is a Passive cable/adapter, the 2nd is an Active cable/adapter.  

A passive cable/adapter does not do a conversion on the protocol and is more limiting. If you have a DisplayPort 1.2 port, you can passively use HDMI 1.4 on the other end; so 4k@30 Hz SDR for video. Passive is most commonly used to get HD audio out of a DisplayPort port connected to a CPU's iGPU and send it to an AVR via HDMI on the other end.  

An active cable/adapter converts the DisplayPort protocol coming into the adapter. This is less limiting and will potentially provide higher bandwidth. For instance, you can use an Active adapter to convert DisplayPort 1.2 to HDMI 2.0 and get 4K@60Hz output, though getting some HDMI 2.0-native features is problematic if they weren't supported by the DisplayPort version to begin with. In our example, since DisplayPort 1.2 does not support HDR, it will not get passed over the adapter.  
SOME oem vendors (hp, dell, levovo) SOMETIMES advertise DisplayPort 1.2, but in reality support 1.3/1.4. When this happens you can use a DisplayPort 1.4->HDMI 2.0 active adapter and get HDR. This support is very spotty, so unless you find accounts of it on the hardware you want to use, don't bet on it.  

Active connectors can also be used to convert DisplayPort 1.4 to HDMI 2.1 and get 4K@120Hz HDR output. This also has its caveats. The adapters require the Display Stream Compression (DSC 1.2) feature to be supported in the GPU for use over DisplayPort. Since this is an OPTIONAL feature to DisplayPort 1.x, do not expect all GPUs with DisplayPort 1.4 to support this. Officially supported GPUS are >= Nvidia GTX 16xx/RTX 20xx or >= AMD RX 5xxx dGPUs.  
Active adapters also do not allow passthrough/bitstreaming of HD audio, only PCM audio.  

USB-C is just a different connector, still carrying the DisplayPort protocol as if it was that connector.  

When buying cables and adapters, please do NOT buy no-name brands. As quality control is low on them and marketing is more often than that mis-leading. Recommended cables and adapters can be found in the hardware section of the [Wiki FAQ](/htpc-wiki/faq). You can also find there what versions of DisplayPort and HDMI are supported on various CPUs/GPUs.  

<!-- Sub-Section -->

### What options are there for 4k @ 120 Hz video output?

Keep in mind we assume a HDMI input will be on your Display (TVs/Projectors, which is our only concern here).  

You will need to have HDMI 2.1 bandwidth on every HDMI device between your HTPC and your Display (GPU, TV, AVR, Switches, etc..). Simply having "HDMI 2.1" does not mean 4k@120 Hz bandwidth will be supported; this is an important distinction, so make sure they state 4k@120 hz support and/or >= 32 Gbps bandwidth (for at least media content) or >= 40 Gbps for gaming.  

Options below for this are ordered from best to worst in terms of stability, reliability, value. This may vary based on your regional pricing and availability.  

Technically, straight HDMI is the best (#1/#2/#3) followed by Thunderbolt->HDMI (#4/#5), USB-C->HDMI (#6) and DP->HDMI (#7). Use of an adapter in #4/#5/#6/#7 assume you have a Display with DSC (Display Stream Compression) support on your HTPC/Display HDMI 2.1 connectors. Media content SHOULD be possible without DSC support, but it's not a given; and VRR gaming will not be supported on any adapter.  
  
1. DiY: Any cpu/motherboard + a discrete GPU w/a 4k@120 Hz HDMI 2.1. e.g. New: Radeon RX 6400, Used: RTX 3050 
2. DiY: An AMD Ryzen 7xxx desktop CPU and respective motherboard that states 4k@120Hz HDMI 2.1. e.g. Ryzen 7600 + ASRock A620I/B650I Lightning Wifi 
3. Pre-built: A Ryzen Mini PC with a 4k@120Hz HDMI 2.1 port. e,g. Minisforum Venus UM760 Pro, ASRock 4x4 7535U 
4. Pre-built: An Intel 11th gen+ Mini PC with a Thunderbolt display out connector and a Thunderbolt->HDMI adapter/cable. e.g. Intel NUC 11/12/13/Lenovo IdeaCentre Mini Gen 8 + [Thunderbolt->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M) 
5. DiY: Intel 12th+ Gen CPU and respective motherboard with a Thunderbolt display out connector out and a [Thunderbolt->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M). Not as good as straight HDMI, but better compared to DP or plain USB-C. This will likely be expensive as these boards are rare. e.g. for an ITX board, look at the Asus ROG STRIX Z690-I GAMING WIFI, ASRock Z690 Phantom Gaming-ITX/TB4 or ASRock Z790 PG-ITX/TB4. 
6. Hybrid/DiY: An Intel 11th gen+ CPU and motherboard w/a USB-C Display Out and a USB-C->HDMI adapter/cable. e.g. ASRock Deskmini B660 + 
[USB-C->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M). 
7. DiY: Intel 12th+ Gen CPU and respective motherboard with a Displayport 1.4 connector and an Active DP->HDMI adapter. This tends to be the least stable option, so we don't recommend it at all. 

<!-- Sub-Section -->

### How do I configure my app/gpu/display for proper color reproduction?

See above sections [Setup For Color Conversion/Reproduction](/htpc-wiki/video#wiki_setup_for_color_conversion.2Freproduction) and [Video Calibration Testing](/htpc-wiki/video#wiki_video_calibration_testing)  

<!-- Sub-Section -->

### Where do I find additional sample video files to test?

[AVS HD 709 Test Patterns](https://www.avsforum.com/threads/avs-hd-709-blu-ray-mp4-calibration.948496/) - For video calibration  

[Jellyfish Video Bitrate Test Files](http://www.larmoire.info/jellyfish/) - 1080p/4k, h.264/HEVC, High/Main (8-bit), Main10 (10-bit), MKV  

[Ideal 4K HEVC test](http://www.larmoire.info/jellyfish/media/jellyfish-140-mbps-4k-uhd-hevc-10bit.mkv) - Max UHD Blu-Ray bitrate - 4k, HEVC, SDR, 140Mbps, 10-bit, 30fps, mp4  

[Our HDR10 Test Videos/Patterns](https://drive.google.com/uc?id=19i_laf6vloxzLic6qOArXt0fLvCpc_qo) - For Basic HDR video calibration  

[Mehanik's Full HDR10 Test Videos/Patterns](https://drive.google.com/drive/folders/1m4IBq0euAxamL9ePgfdFuf8_5nLcRwHA) - For Advanced HDR video calibration  

[Ideal 4K HEVC HDR10 test](https://4kmedia.org/samsung-hdr-picture-quality-uhd-4k-demo/) - High UHD Blu-Ray bitrate - 4k, HEVC, HDR10, 50-90Mbps, 10-bit, 30fps, mp4  

[Other 4K Media Test Files](https://4kmedia.org) - 4k, h.264/HEVC, HDR10/DV, TS/MKV/MP4, 24-60fps  

[Other Media Test Files](https://test-videos.co.uk/) - 360p/720p/1080p h264/HEVC/AV1/VP8/VP9  

<!-- Section -->

## Accessories

**HDMI extenders**  

4k@60Hz + USB: [OREI](https://www.amazon.com/dp/B0BPVX4VYT)  

4k@60Hz + IR/Audio: [OREI](https://www.amazon.com/dp/B0BPW1ZC1B)  

**HDMI Splitters**  

4k@120Hz: [Monoprice Blackbird](https://www.monoprice.com/product?p_id=44436)

