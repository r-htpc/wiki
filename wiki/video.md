---
description: Information on how to configure, calibrate, and explanation of VIDEO between your HTPC and Display
---

# Video Setup Guide

*This page is best viewed with a PC web browser.*  

<!-- Section -->

## Technologies

Please read the Video Formats and Transports sections before you embark on the Setup section below it, so you understand the terms and concepts mentioned.  

For simplicity, the term "HTPC" here means a PC, not a streaming device, like a Roku/Fire TV/etc, except where  noted.  

<!-- Sub-Section -->

### **Video Formats/Codecs**

x264: Also known as h.264/MPEG-4 AVC. A very common lossy video compression codec. Used in Netflix, newer HD blu-ray discs and ATSC 1.0 OTA. Optimal for resolutions <= 1080p.  
x265: Also known as h.265/MPEG-H HEVC. The successor to AVC with better, but still lossy, compression. Used in 4k Netflix, UHD blu-ray discs and ATSC 3.0 OTA. Optimal for resolutions >= 1440p.  
Xvid/Divx: Also known as h.263/MPEG-4 Part 2. Xvid is an open-source version. An old compression codec commonly used in AVI and Divx containers.  
VC-1: Used in newer HD blu-ray discs  
VP9: A compression codec used on Youtube  
AV1: A modern, lossy compression codec currently with limited support. The successor to HEVC and VP9. Sparse usage on Youtube/Netflix  
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

### **Video Frame rates/Bit rates**

**Frame rates** 

Commonly known as FPS or Frames Per Second. Do not confuse this with Refresh Rate; they are related, but not the same thing. Frame rate refers to Content,
Refresh rate refers to Displays. The refresh rate should be either equal to the frame rate or greater than it by an whole number multiplier (120Hz for 24fps (5x)). A refresh rate greater than it by anything else (60 Hz for 24 fps (2.5x)) can cause a [Judder](https://www.rtings.com/tv/tests/motion/24p) effect.

FRAME RATE|USE|NOTES
:--|:--|:--
23.976/24|Movie content (common) - Local or Streaming, Youtube (rare)|Usually upconverted to 60i on TVs through a process known as 2:3/3:2 pulldown.
25|TV content - Local, Streaming or Broadcast TV (outside US/Central America/SE Asia), Youtube (rare)|European standard used in PAL color-encoding for 576i
29.97/30|TV content (common) - Local, Streaming or Broadcast TV (US/Central America/SE Asia), Youtube (rare)|Standard used in NTSC color-encoding. Interlaced to 60 fps for TV
48|Movie content (very rare)|< 10 movies
60|Youtube [TV] content (common), Broadcast TV/Streaming - Live Events, Movie content (very rare)|60i (cable/sat), < 10 movies

**Bit rates** 

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
HDMI 2.1: Digital. Up to 48 Gbps. 4K @ 144 Hz. HDR+  
Displayport 1.2 (native): Digital. Displayport on both ends. 20 Gbps. 4K @ 60 Hz  
Displayport 1.4 (native): Digital. Displayport on both ends. 32 Gbps. 4K @ 120 Hz. HDR  
Displayport (Alternate mode): Digital. Displayport/USB->HDMI cable/adapter  
[HDCP](https://en.wikipedia.org/wiki/High-bandwidth_Digital_Content_Protection): Copy-protection/DRM required for Disc playback and most commerical streaming services, in all devices of video chain. Supported on DVI, HDMI, DP interfaces. 2.x required for 4k media. 

<!-- Sub-Section -->

### **Video Metadata/Color Technologies**

**HDR Types**

HDR10: Very common. Very compatible. Static Metadata. 400-4000 cd/m2. 10-bit color.  
HDR10+: Not common. Dynamic Metadata. 1000-4000 cd/m2. 10-bit color. **No passthrough on an HTPC**  
Dolby Vision: Very common. Not very compatible, esp. with local content. Dynamic Metadata. 1000-4000 cd/m2. 12-bit color. **No passthrough on an HTPC**  
HLG: Not common. No metadata. SDR & HDR in same signal. 1000 cd/m2 nominal. 10-bit color.  
[Wiki:FAQ:What is HDR video and what do I need to take advantage of it?](/wiki/faq#what-is-hdr-video-and-what-do-i-need-to-take-advantage-of-it)  

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
 - eGPU: A graphics card external to the HTPC, connected to it via USB/Thunderbolt/Oculink.  
2. Display
 - TV  
 - Projector  

<!-- Sub-Section -->

### **Video Software**

See also: [Audio Software](/wiki/audio#audio-software)  

**Media Servers**

1. [Plex](https://plex.tv) - Media server software that streams content out to clients. Distinguishing features include:  
 -  Support for Windows, Linux, Mac, Docker 
 -  Support for live tv via tv tuners  
 -  Automatic scanning of video content directories  
 -  Automatic retrieval of metadata content (posters, descriptions, trailers) from the internet  
 -  Real-time transcoding video/audio down to other containers, codecs, resolutions and bitrates via CPU/GPU. 
 -  Streaming of video content to remote video clients  
 -  Support for playback via windows, linux and web browser clients  
 -  Additional pay-for features such as Remote playback, Hardware Transcoding, Intro skip, Credit skip, DVR, Premium Music, and Offline Downloads  
 -  HDR tonemapping, Media collections, Subtitle support
 -  Closed source 
2. [Jellyfin](https://jellyfin.org)  
 -  Decent media server alternative to Plex, but not as polished or supported across clients. 
 -  Support for Windows, Linux, Mac, Docker 
 -  GPU transcoding support is free. 
 -  Streaming of video content to remote video clients requires direct access to server. 
 -  HDR tonemapping support
 -  Open source
3. [Emby](https://emby.media)  
 -  Decent media server alternative to Jellyfin/Plex, but not as polished, or supported across clients for free.
 -  Support for Windows, Linux, Mac, Docker 
 -  Additional pay-for features such as Hardware Transcoding, DVR, Offline Downloads and Sync.
 -  Closed source
4. [DLNA](https://en.wikipedia.org/wiki/DLNA)  
 -  Simple, widely supported across hardware and platforms. Varying degress of features (metadata, transcoding, etc..)
 -  Built into Windows (media streaming); Universal Media Server, Serviio  

**Players**

1. [Kodi](https://kodi.tv) - An open source media player/center.  
 - Support for Windows, Linux, Mac, Android  
 - Automatic scanning of video content directories  
 - Automatic retrieval of metadata content (posters, descriptions) from the internet  
 - Extensive plug-in support  
 - 4K/[HDR support](/wiki/hdr), Subtitle support  
 - MadVR integration  
 - Keyboard/remote support 
2. [Plex HTPC](https://www.plex.tv/media-server-downloads/?cat=plex+htpc&plat=windows#plex-app) - A media player that interfaces with the Plex Media Server and plex.tv video content  
 - Support for Windows, Linux, Mac, Android  
 - 4K/[HDR support](/wiki/hdr), Subtitle support  
 - Keyboard/remote support 
3. [Jellyfin Media Player](https://github.com/jellyfin/jellyfin-media-player/releases) - A media player that interfaces with the Jellyfin media server  
 - Support for Windows, Linux, Mac  
 - 4K/[HDR support](https://forum.jellyfin.org/t-4k-hdr-client), Subtitle support  
 - Keyboard/remote support in "TV" mode 
4. [VLC](https://www.videolan.org/vlc/)  
 - Support for Windows, Linux, Mac, Android  
 - 4K/[HDR support](/wiki/hdr)  
 - DVD/Blu-ray folder support  
5. [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases)/[MPC-HC](https://github.com/clsid2/mpc-hc/releases/)  
 - Support for Windows  
 - Extensive feature-set
 - MadVR/MPC VR integration  
 - 4K/[HDR support (via MPC VR/MadVR)](/wiki/hdr)  
 - Subtitle support  
 - DVD/Blu-ray folder support  
6. [JRiver Media Center](https://jriver.com/)  
 - Support for Windows, Mac, Linux  
 - Automatic scanning of video content directories  
 - Automatic retrieval of metadata content (posters, descriptions) from the internet  
 - MadVR integration  
 - 4K/HDR support, Subtitle support  
 - Keyboard/remote support 
 - Commercial
7. [MPV](https://mpv.io)  
 - Support for Windows, Linux, Mac, Android  
 - Minimal GUI  
 - 4K/HDR support  
8. PowerDVD  
 - DVD/Blu-ray/UHD Blu-ray disc support; Ultra version <= v22.0.3214.62 for UHD  
9. PotPlayer  
 - MadVR integration  
 - 4K/HDR support (via MadVR)  
 - Closed source  

**3rd Party**

1. [MediaInfo](https://mediaarea.net/en/MediaInfo) - Extremely useful tool for getting various video & audio information (codecs, formats, etc..) on media files  
2. [MPC VR](https://github.com/Aleksoid1978/VideoRenderer) - Simple video renderer used to enable HDR passthrough, HDR tonemapping, Resolution/Chroma upscaling, Dithering  
3. [MadVR](https://wiki.jriver.com/index.php/MadVR_Expert_Guide) - Advanced video renderer for HDR passthrough, [HDR tonemapping](https://madshi.net/madVRhdrMeasure113.zip), Resolution/Chroma upscaling, Dithering, Resolution/Refresh Rate Switching.
 - [Stable base install](http://madshi.net/madVR.zip) / [Non-expiring add-on - beta](https://madshi.net/madVRhdrMeasure113.zip) / [Expiring add-on - test builds](https://www.videohelp.com/software/madVR)   
5. SVP - Used to upscale frate-rates for video smoothing  
6. [K-lite](https://codecguide.com/download_kl.htm) - Codec pack including various video software  
 - Video/audio codecs  
 - Video/audio filters/splitters/mixers  
 - MPC VR, MadVR  
6. [LAV Filters](https://github.com/Nevcairiel/LAVFilters) - ffmpeg based DirectShow media software including:  
  - Splitters, Decoders, Filters, Mixers and Compressors  
  - Automatic stream selection
7. [Media Hoarder](https://media.hoarder.software/) / [tinyMediaManager](https://www.tinymediamanager.org/) - Media/Metadata Management  
8. [Handbrake](https://handbrake.fr) - Media Converter. See Also: [FAQ:How can i rip my DVD/Blu-ray discs and what are some good quality settings to use?](/wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use)  
9. Virtual CloneDrive - Mount ISO files for disc playback support  

<!-- Section -->

## Setup

### **Introduction**

**Hardware Setup**  

See the [AUDIO Setup Guide](/wiki/audio) for different ways of connecting your HTPC to a display and sound system.  

**Software/OS Setup**  

Make sure the video driver for your GPU is installed, updated from the GPU vendor, and working.  

Set up your app/gpu driver/tv settings for color reproduction. See [section below](/wiki/video#setup-for-color-reproduction).  

Run video calibration tests to make sure the above setup is correct. See [section below](/wiki/video#video-calibration-testing).  

Run motion calibration tests for judder/stutter. See [section below](/wiki/video#motion-calibration-testing).  

Configure your video player application for hardware decoding. See [section below](/wiki/video#application-specific-setup-for-hardware-decoding).  

OPTIONAL: Configure your video player application for additional video features. See [section below](/wiki/video#additional-video-feature-testing).  

<!-- Sub-Section -->

### **Setup For Color Reproduction**

You will use this section to set up the resolution, refresh rate, bit-depth and color format for your GPU and Display.

While researching setup of your devices you may have come across confusing terms like YCbCr, RGB, RGB full/limited, black level.  

First, let's get YCbCr and RGB out of the way. These are color spaces for encoding content. RGB treats blacks, whites and colors equally. YCbCr treats blacks and whites differently than colors, in that it compresses colors such that our eyes can't really tell the difference between it and RGB; this saves bandwidth.  
YCbCr is common for video content and will get converted to RGB in your media application. RGB is common for games and the desktop. Therefore everything coming out of your media application/desktop to the GPU should be RGB. 

Now, to RGB full/limited. In short, RGB full/limited is just different numbering systems to apply to the range of white to black. RGB Full denotes 0 as Black and 255 as White. RGB Limited denotes 16 and below as Black and 235 and above as White.  

What makes this confusing is a setting of Full or Limited can be on multiple pieces of your system, more specifically:  

1. The Application (The video renderer (madVR/MPC VR/EVR CP) in what you're using to play/decode/render your content, Kodi, Plex, MPC, etc..)  
2. The GPU driver (nvidia, amd, intel, etc..)  
3. The Display (TV, Projector)  

If you set each piece in the wrong combination, whites and blacks will look wrong, colors will be washed out and/or shadows/details will be diminished.  
Here's what should be set for the 3 pieces above, depending on your scenario, but use #1 first, where at all possible.  

- Scenario #1 - PC Recommended: 
  - Application: Range: **Full (0-255)**, Bit depth: auto/\<display bit depth\> 
  - GPU: Color/Pixel Format: RGB, Range: Full  
  - Display: Color Space: RGB/Native, Range: **Full**.  
- Scenario #2 - PC Alternate: 
  - Application: Range: **Limited (16-235)**, Bit depth: auto/\<display bit depth\>  
  - GPU: Color/Pixel Format: RGB, Range: Full  
  - Display: Color Space: RGB/Native, Range: **Limited**  
- Scenario #3 - Media device (roku, shield, fire tv) video content on a TV:  
  - Application: Limited (16-235), where available  
  - GPU: Color Space: YCbCr/YUV 422 12-bit  
  - Display: Limited  

To confuse things even more, sometimes Full and Limited are called by other names. We urge you to read a primer on calibration settings which explains more of the terms you'll find in your Display and what they're called for each major mfgr. The page at [rtings.com](https://www.rtings.com/tv/learn/how-to-calibrate-your-tv) is a good one to start with. If you still can't figure out what ranges are available on your Display, **assume it's in Limited range by default** unless you change it (like put in PC mode) or your manual says otherwise.  

**After all that, make the changes based on the above 3 scenarios. As mentioned above, when in doubt, use Scenario #1, as exampled with the following for a PC**

1. Change your video application's renderer to a Range of Full (0-255). This is the default for all renderers (madVR/MPC VR/EVR CP) unless otherwise changed. Change Bit depth to auto  
2. Change your Display to:
 - If for 4k, Have a HDMI signal format of *UHD Deep Color/Input Signal Plus/Enhanced*
 - Have a color space of RGB/Native (where available) or Auto. Change the input range to Full. As a last resort, put your Display in PC or Game Mode. This will remove a lot of Display processing options, so if this is not desired, you may want to use Scenario #2's Limited settings for this step and step #3.  
3. Change your GPU driver settings to a Resolution, Refresh Rate, Color/Pixel Format, Color Depth based on the below for your video interface. Only use ALT: if you know what you're doing.
 - HDMI 1.4: 3840x2160, 30 Hz, RGB, 8-bit : 1920x1080, 120 Hz, RGB, 8-bit (ALT: 10-bit w/color format YCbCr 420) 
 - HDMI 2.0: 3840x2160, 60 Hz, RGB, 8-bit (ALT: 10-bit w/color format YCbCr 420) 
 - HDMI 2.1: 3840x2160, 120 Hz, RGB, 10-bit
 - Displayport 1.2: 3840x2160, 75 Hz/8-bit - 60 Hz/10-bit, RGB
 - Displayport 1.4: 3840x2160, 120 Hz, RGB, 10-bit
4. Run the Contrast, Black Level and Gradient tests from [Lagom LCD Tests](http://www.lagom.nl/lcd-test/)

*The above are realistic and recommended settings for each video interface. Higher refresh rates may be possible (e.g. 144 to 165 Hz), where supported by the Display and contingent on [proper cables and optimal video cable length](/wiki/components#video-cablesadapters) and/or a single, direct GPU->Display connection. They are not recommended for media consumption due to stutter/judder problems.*

<!-- Sub-Section -->

### **Video Calibration Testing**

This section is UNDER CONSTRUCTION.  

We know it is tempting to install and configure every software you want to use right away and get on to playing content; but doing everything all at once usually leads to problems which become hard to diagnose once you've added so many software and configuration layers on top of your base OS.  
As such, it is highly recommended to run video calibration tests before you play real content so you know you've set up the combination of your app/gpu/display properly to get the proper colors, whites/blacks, and motion for the video content you will be playing.  

To do this, you should
 
1. Set the proper color conversion/reproduction settings, if you haven't already, from the [Setup for Color Reproduction](/wiki/video#setup-for-color-reproduction) section above.  
2. Calibrate your display using [hardware](https://calibrite.com/us/product/display-plus-hl/) and [software](https://store.portrait.com/consumer-software.html) means if you can afford it. Read [this article](https://tftcentral.co.uk/articles/lg-oled-tv-calibration-guide-autocal-and-hardware-calibration) for the basics; else, do a basic calibration of your display in your display settings/OS. In Windows, Start->Color Management->Advanced->Calibrate Display
3. Choose a video player application to test with. We recommend [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases) on Windows and [Kodi](https://kodi.tv/download/linux/) on Linux.   
4. **Disable** Hardware Decoding/Acceleration (DXVA, D3D11, NVDEC, pixel shaders etc..) in your video player application, to minimize the chance of the GPU decoder/renderer messing up colors, blacks and whites. You will re-enable it later. The options to do so are different depending on your media player. It should be set to Software/None/Acceleration disabled/etc or disable by codec; see the location for the option(s) in the [Hardware Decoding section](/wiki/video#application-specific-setup-for-hardware-decoding) below.      
5. Download calibration media like [AVS HD 709](https://www.avsforum.com/threads/avs-hd-709-blu-ray-mp4-calibration.948496/). Get the MP4 version. At the minimum, extract the tests from the 'Basic Settings' and 'Misc Patterns->A' folder.  
6. Read the [AVS manual](https://www.w6rz.net/avshd709/Patterns-Manual.pdf) and then run the calibration tests in your video player application.  
7. You're not looking for smooth playback here but proper colors, contrast and balance. If everything in the tests look good, **Enable** Hardware Decoding/Acceleration in your media player as per the [section](/wiki/video#application-specific-setup-for-hardware-decoding) below. If everything does NOT look good, you messed something up in #1/#2. Go back and re-check/re-try.  
8. Re-run the AVS calibration tests.   
9. If everything in the tests look good, start playing some test content. Use known-good content in our [test files](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) section below.  
  - Jellyfish Codec Tests - Start here just to test common codecs are using HW acceleration properly under your GPU.
  - Ideal 4K HEVC test - Represents the max bitrate (120 Mbps) and frame rate (30 fps) you're likely to see from local content
  - Ideal Youtube tests - Represents the max bitrates and frame rate (60 fps) you're likely to see from Youtube content
  - Jellyfin Video Bitrate Tests - Represents the max frame rate (60 fps) you're likely to see for Cameras/0.1% movie/Broadcast/Sports content, at varying bitrates. These would be rare and niche depending on use-case.
10. If you're dropping frames from the content, consult the [dropping frames](/wiki/video#why-is-my-video-playback-stuttering-andor-dropping-frames) question below before moving on.
11. Return to the Software/OS Setup section above for additional testing.

<!-- Sub-Section -->

### **Motion Calibration Testing**  

This section is UNDER CONSTRUCTION.  

You will first run a test for the presence of motion problems like stutter. You will do this under a no-judder condition where the content frame rate and display refresh rate match. After that you will test for [judder](https://www.rtings.com/tv/tests/motion/24p) itself and how bad it is for you subjectively.  

1. Set your display (through the GPU driver) to a specific refresh rate equal to the content you want to test. e.g. 23Hz for 23.976fps content, 24Hz for 24fps, etc..
2. Test that the refresh rate is set correctly and consistently using [this page](https://www.testufo.com/refreshrate).
3. If testing local content, choose a video player application to test with. We recommend [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases) on Windows and [Kodi](https://kodi.tv/download/linux/) on Linux.
4. Play test content and look for any observable motion problems.
   - Local: [Test Files -> Frame Rate Tests](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) 
   - Youtube: [24p content](https://www.youtube.com/watch?v=oy8wNzOGVmc)/[25p content](https://www.youtube.com/watch?v=Ou3QXsTro7A)/[60p content](https://www.youtube.com/watch?v=RgGwWN9EC8g) 
5. If you see a motion "problem", it's not judder, and likely some form of [stuttering](https://www.youtube.com/watch?v=CuEZIJDEQyo&t=1s). Some stutter is not necessarily something that needs to be solved as it can just be a time-consistent symptom of low frame rate content. If it looks like more than that, see [this section](/wiki/video#why-is-my-video-playback-stuttering-andor-dropping-frames) below before you move on; then repeat the tests.  
6. If you don't see a motion problem, and you plan to play content on a refresh rate that's NOT a multiple of your content frame rate (e.g 24p/25p on 60 Hz, 24p on 25Hz/50Hz), you should continue on to test for [judder](https://www.rtings.com/tv/tests/motion/24p).  
7. Set your display (through the GPU driver) to the desired non-multiple refresh rate. e.g. 60 Hz for 24 fps content.  
8. Test that the refresh rate is set correctly and consistently using [this page](https://www.testufo.com/refreshrate).  
9. Play test content and look for any observable judder.
   - Local: [Test Files -> Frame Rate Tests, Judder Tests](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) 
   - Youtube: [24p content](https://www.youtube.com/watch?v=oy8wNzOGVmc)/[25p content](https://www.youtube.com/watch?v=Ou3QXsTro7A)
10. [Judder](https://www.rtings.com/tv/tests/motion/24p) will likely be present; watch [this video](https://www.youtube.com/watch?v=CuEZIJDEQyo&t=1s) to see what it will look like. What's important is how bad it is and if it's something that's too distracting that you can't ignore. If you can't ignore it, see the [section](/wiki/video#how-do-i-fix-judder-on-my-htpc) below and repeat the tests.  
11. Return to the Software/OS Setup section above for additional testing.

<!-- Sub-Section -->

### **Additional Video Feature Testing**  

1. Make any additional video setting changes you desire ([enabling HDR, changing renderers, upscaling](/wiki/hdr), [Resolution/Refresh Rate Switching](/wiki/video#application-specific-setup-for-resolutionrefresh-rate-switching), etc..) and play [test content](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) again. 
2. If everything in the tests do NOT look good, either there's something messed up in your GPU color conversion/decoding, your display device is limiting you (e.g. HDR luminance/tonemapping), or your GPU/renderer is limiting you (e.g. aggressive post-processing); perform a full calibration from the Software/OS section above if you haven't already done so, and/or seek help on the sub.  

<!-- Sub-Section -->

### **Application-Specific Setup For Hardware Decoding**

Most video players have hardware decoding support built-in.  

Configuration usually involves a single toggle on the simple side, or, on the advanced side, choosing between DVXA/D3D11/Quicksync and/or choosing your proper GPU Device. Make sure your GPU Device supports hardware decoding for the format(s) you're trying to play. See the [GPU Feature Set Matrix](/wiki/components#gpusgraphics) of the Wiki.  

If configured correctly, CPU Usage should be low during playback, while GPU Usage (Video Decode) should be non-0. If GPU Video Decode is 0, then hardware decoding is not being used.

BROWSERS/STREAMING SERVICES:  
1. Make sure your service supports the video codec/resolution you want to play. See: [Wiki:FAQ:What resolution and audio is supported on streaming service X?](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x)
2. If 4k, make sure you have the proper hardware and dependency software. See [here](/wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility).
3. If applicable, install the app for your service from the Microsoft store or use a browser listed in step 1's link for the desired res/audio.
4. Make sure Graphics accleration and DRM is enabled in your browser. Search for "acceleration" or "performance" in your browser's settings page for acceleration. "DRM" or "Widevine" for DRM. Restart your browser after any change.  
5. If HDR, see: [Wiki:HDR Setup Guide:Streaming Content (Netflix, Youtube, etc..)](/wiki/hdr#streaming-content-netflix-youtube-etc)  
6. Test your browser's video capabilities with [Dolby's capabilities test website](https://ott.dolby.com/codec_test/index.html)  

MPC-BE:  
1. View->Options->Internal Filters->Video Decoders->Video Decoder Configuration
   - Codecs: <all checked\>
   - Preferred Decoder: 'D3D11, DXVA2' (Win 8+) or DXVA2 (copy-back) (others)

MPC-HC:  
1. View->Options->Internal Filters->Video Decoder: Hardware Decoder to use: D3D11 (Win 8+) or DXVA2 (copy-back) (others)  
2. View->Options->Internal Filters->Video Decoder: Hardware Device to use: Automatic (if D3D11) or Your_GPU_Device (DXVA2)

VLC:  
1. Tools->Preferences->Input/Codecs->Hardware-accelerated decoding: Direct3D11 (Win 8+) or DirectX (others)

Plex:  
1. Plex HTPC/Plex Media Player 
  - Settings->Video->Use Hardware Decoding: Enable  
2. Plex for Windows
  - Settings->Player->Use Hardware Decoding: Enable  

Kodi:  
1. Settings->Player->Change to "Advanced" config view  
2. Settings->Player->Videos->Render Method: DXVA/Automatic  
3. Settings->Player->Videos->Allow hardware acceleration - DXVA2: Enable  
4. Press 'O' during playback to test for (HW) video decoder  
  
Potplayer: F5 Key->Filter Control->Video Decoder->Built-in Video..->Use DXVA: Enable, Codecs your GPU supports: VLD  

LINUX:
1. Ideally use Mint, Arch, PopOS or another distro with VA-API support (otherwise see [here](https://rpmfusion.org/Howto/Multimedia))
2. Install gpu driver and libva-\<gpu\>-driver packages for your distro.
3. Configure player to use VA-API

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
   ------ 01: [ 23 ] @ \<your res\>  
   ------ 02: [ 24 ] @ \<your res\>  
   ------ 03: [ 50 ] @ \<your res\>  
   ------ 04: [ 29 ] @ \<your res\>  
   ------ 05: [ 30 ] @ \<your res\>  
   ------ 06: [ 50 ] @ \<your res\>  
   ------ 07: [ 59 ] @ \<your res\>  
   ------ 08: [ 60 ] @ \<your res\>  

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
5. Web Browsers: Not available  

<!-- Sub-Section -->

### **Application-Specific Setup For HDR/Scaling**

[HDR Setup Guide](/wiki/hdr)  

<!-- Section -->

## Common Questions

<!-- Sub-Section -->

### What kind of video is supported for streaming services?

See [Wiki:FAQ:What resolution and audio is supported on streaming service X?](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x)

<!-- Sub-Section -->

### How can i play my DVD/Blu-ray discs on my HTPC?

Ideally, you shouldn't; especially for UHD/4K, as the [system requirements are so restrictive](/wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility) to make it not worth-while.  

You should rip your discs to digital files per [Wiki:How can i rip my DVD/Blu-ray discs and what are some good quality settings to use?](/wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use)  

If you must have menus, which is presumably the reason you want disc playback, create an unencrypted ISO of it.  
 1. If UHD Blu-Ray, make sure [you have a UHD Friendly drive](/wiki/components#optical-drives)
 2. Install and run [MakeMKV](https://www.makemkv.com/)
 3. Insert your disc
 4. Create the backup
    - If DVD:
      - Click the disc backup icon in the Toolbar. This will create an unecrypted ISO. Specify the output path for it
    - If FHD/UHD Blu-ray:
      - Click the disc backup icon in the Toolbar. This will create an unencrypted folder structure. Specify the output path for it
      - Use [ImgBurn](https://www.imgburn.com/index.php?act=download) to create an ISO file from the unencrypted folder
 5. Play the ISO with a compatible player; these are:
    - Kodi (w/[Java 8](https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html) for Blu-Ray)
    - VLC
    - MPC-HC/MPC-BE
    - JRiver
    - If you have problems opening the ISO with a player, mount the ISO with [CloneDrive](https://www.majorgeeks.com/files/details/virtual_clonedrive.html) first and open the folder structure

If you must have disc playback:
 1. DVD: Kodi/MPC-BE/VLC, [Microsoft DVD player](https://apps.microsoft.com/detail/9nblggh2j19w?activetab=pivot%3Aoverviewtab&rtc=1&hl=en-us&gl=US#activetab=pivot:overviewtab), [Xreveal](https://www.xreveal.com/) + Media player above
 2. FHD Blu-Ray: [Leawo Blu-Ray Player](https://www.leawo.com/blu-ray-player/), [Xreveal](https://www.xreveal.com/) + Media player above
 3. UHD Blu-Ray: *Official UHD Drive*: [CyberLink PowerDVD Ultra <= v22.0.3214.62](https://www.cyberlink.com/products/powerdvd-ultra/features_en_US.html). *[UHD-Friendly Drive](/wiki/components#optical-drives)*: [Xreveal](https://www.xreveal.com/) + Media player above
 4. Make sure you meet audio/video chain restrictions: [HDCP](https://en.wikipedia.org/wiki/High-bandwidth_Digital_Content_Protection) 1.x for DVD, HDCP 1.3 for FHD Blu-Ray, HDCP 2.2 for UHD Blu-Ray; in all devices of the video chain (Drive, GPU, Video Cable, Display)  

See our [Optical Drive](/wiki/components#optical-drives) section of the Hardware Components page for drive selection  

<!-- Sub-Section -->

### Why won't my video signal remain stable?
### Why doesn't my video signal go up to the stated resolution/refresh rate?

1. You may be using a bad, poor quality, or inadequately speced HDMI cable/adapter. Use a [better one](/wiki/components#video-cablesadapters)
2. Your total HDMI cable length may be too long for the resolution/refresh you want to use. Use [shorter cables or cables designed for long runs](/wiki/components#video-cablesadapters)
3. If for 4k: Your Display's HDMI port may not be set to the proper signal format. You should set it to *UHD Deep Color/Input Signal Plus/Enhanced* on the Display (setting name dependent on TV mfgr). If a Sound System is in-between your HTPC and TV, you should set your Sound System's HDMI port to a HDMI Format/4k Signal Format of *Enhanced*, where available.
4. You may have a bad HDMI port on your Display, GPU, or an in-between Sound System. Try a different port.
5. You're using too many cable segments in the HDMI cable run from the HTPC to Display. You should limit the amount of segments to 2. HTPC->TV would be 1. HTPC->AVR->TV would be 2. HTPC->AVR->Wall jack->TV would be 3. If you have a wall jack behind the TV AND behind the AVR, that's 4. You can *usually* make up for using more segments with shorter/better cables or brush plates instead of wall jacks.
6. You GPU driver may be corrupted. Run [DDU](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html) to remove it fully and then re-install the driver.
7. You're overclocking your GPU or have a bad GPU.
 

<!-- Sub-Section -->

### What are the best ways for scaling video?

Video scaling algorithms are available to configure in the [MPC VR](/wiki/hdr#mpc-be--mpc-video-renderer) and [madVR](/wiki/hdr#mpc-hcmpc-be--madvr) video renderers. Our HDR setup guide has basic instructions for player/renderer combos.

From Worst to Best quality (and generally least resource intensive to most) the algos are:  

Nearest Neighbor, Bilinear, DXVA, Cubic (Mitchell Netravali), Cubic (BiCubic), Catmull-Rom, Lanczos 2/3, Spline, Jinc, SSIM (downscale), super-xbr, NGU Standard (>= doubling), NGU Sharp (>= doubling). The Anti-Ringing/AR option added on to any algo is ideal, where available.  

These are OBJECTIVE rankings, and not SUBJECTIVE. Visual preferences are subjective i.e. different for each person. Test the algos to find the sweet spot for your own visual and GPU load/noise preferences. Do not go past the [recommended algos for your particular GPU](/wiki/hdr#madvr-performance-settings-per-gpu) without extensive performance testing.  

[MPC VR](/wiki/hdr#mpc-be--mpc-video-renderer) will allow you to go up to the Jinc algo. [madVR](/wiki/hdr#mpc-hcmpc-be--madvr) to the NGU Sharp algo.  

Any algo beyond **Jinc** will produce diminishing returns compared to the amount of load and noise it subjects your GPU to and may be detrimental to your HT listening environment.  

If you have an Nvidia RTX 30+ series GPU you can also use RTX Super Resolution in the MPC VR renderer and in Windows in general for non-DRM streaming sites, like Youtube. It's quality will be somewhere around the Jinc algo, so is not a replacement for the best madVR.

<!-- Sub-Section -->

### Why is my video playback stuttering and/or dropping frames?

First, make sure what you're experiencing is actually stutter and not judder. Watch [this](https://www.youtube.com/watch?v=CuEZIJDEQyo&t=1s) video.  

1. Your content is poorly encoded or has a frame-rate that is mis-matched from your display's refresh-rate. Test with [known-good test files](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) of varying frame-rates and/or make sure your refresh-rate is a whole number multiple of the frame-rate. 
2. You're using an OLED TV, which can cause stutter due to the nature of the tech. Test with [Motion Interpolation enabled](https://www.rtings.com/tv/tests/motion/motion-interpolation-soap-opera-effect#related-settings) on it at various levels. 
3. You haven't configured your video player to use your GPU to hardware decode video. See application-specific setup above.
4. If you have an Nvidia GPU, in Nvidia Control Panel -> Manage 3D Settings, Set Vertical Sync: ON, Low Latency Mode:OFF, Power Management Mode: Prefer Maximum.
5. If you have an AMD GPU: In Radeon Settings, Display -> Radeon FreeSync: OFF, Graphics -> Enhanced Sync: OFF, Wait for Vertical Refresh: ON, either globally or create a app profile for your video player  
6. You've configured your Windows power plan or Video driver power settings to balanced/power saving. Test with your Windows power plan set to High Performance. Test with your Video driver power management set to maximum performance.
7. Your GPU doesn't support hardware decoding for the video codecs you're trying to play and your CPU isn't powerful enough to software decode them. Determine what video codec you're attempting to decode (using something like [MediaInfo](https://mediaarea.net/en/MediaInfo)) and then see the GPU section of the Hardware Components Guide for what codecs are supported by your GPU. Buy a better [CPU](/wiki/components#cpus) or [GPU](/wiki/components#gpusgraphics).
8. You're running on the edge of what your CPU/GPU can do performance-wise for the video bitrates you're trying to play. The higher the video bitrate, the more stress put on your CPU/GPU. Audit the GPU tab of Task Manager. Set your video player's process priority to Above Normal. Play lower bitrate videos. Buy a better [CPU](/wiki/components#cpus) or [GPU](/wiki/components#gpusgraphics).
9. You're doing too much post-proccessing with your video renderer (MadVR, MPC, EVR, etc..). Do less post-processing - Lower/Disable upscaling/downscaling/dithering techniques (nearest-neighbor/bilinear).  Use a more efficient renderer. Buy a better [GPU](/wiki/components#gpusgraphics).
10. You're running your RAM in single-channel mode or haven't dedicated enough RAM to your iGPU. Run 2+ sticks of RAM in dual-channel mode for the best performance. If using an iGPU, dedicate as much RAM to it, in your BIOS, where possible.
11. Your CPU/GPU is doing too much work in the background. Audit Task Manager (Windows)/System Monitor (Linux) and disable background tasks and/or processes using the CPU/GPU (updates, antivirus, disk indexing).
12. Your video driver is out of date. Update it and/or re-install the driver clean after running [DDU](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html).
13. You have Dynamic Refresh Rate enabled in Windows. Disable it.
14. Your video player isn't good/good at playing the video codec(s) you're trying to play. Try a different one (MPC-BE, MPC-HC, Kodi, VLC, Jriver, MPV)
15. Use the [SVP (Smooth Video Project)](https://www.svp-team.com/) filter to up-convert the content's fps (e.g. 23.976 fps to 60 fps) before it gets to the display; this is Motion Interpolation, and its effect is unliked by some. Alternatively, you can try madVR's frame blending feature in the rendering->smooth motion section of its settings. 

<!-- Sub-Section -->

### How do I fix judder on my htpc?

First, make sure what you're experiencing is actually judder and not stutter. Watch [this](https://www.youtube.com/watch?v=CuEZIJDEQyo&t=1s) video.  

If you do have judder, then do one or more of the following..  

1. Your content is poorly encoded. Test with [known-good test files](/wiki/video#where-do-i-find-additional-sample-video-files-to-test) of varying frame-rates and/or make sure your refresh-rate is a whole number multiple of the frame-rate. 
2. Configure your video players to switch the video card refresh rate automatically to match the content being played. See [section above](/wiki/video#application-specific-setup-for-resolutionrefresh-rate-switching)
3. Configure your video card settings to run at a refresh rate that matches the bulk of the content you play. e.g. 23 Hz for 23.976 fps content.
4. If you can't/won't do #2 or #3. Set your refresh rate to a number that divides equally into the fps of the bulk of the content you play. e.g. 120 Hz (for 24/30/60 fps).
5. If #3/#4 doesn't work, configure Judder reduction in your TV settings. Some TVs do this automatically. This may be called ["Cinema Screen", "Motion Flow/CineMotion", "Judder Reduction" or "Film Mode"](https://www.rtings.com/tv/tests/motion/24p#related-settings). As a worst case, test with Motion Interpolation enabled at various levels. 
6. If you have an Nvidia GPU, in Nvidia Control Panel -> Manage 3D Settings, Set Vertical Sync: ON, Low Latency Mode:OFF, Power Management Mode: Prefer Max/Adaptive/Normal.
7. If you have an AMD GPU: In Radeon Settings, Display -> Radeon FreeSync: OFF, Graphics -> Enhanced Sync: OFF, Wait for Vertical Refresh: ON, either globally or create a app profile for your video player  
8. Use the [SVP (Smooth Video Project)](https://www.svp-team.com/) filter to up-convert the content's fps (e.g. 23.976 fps to 60 fps) before it gets to the display; this is Motion Interpolation, and its effect is unliked by some. Alternatively, you can try madVR's frame blending feature in the rendering->smooth motion section of its settings. 
9. Use a media device instead that can do automatic Refresh Rate Switching. Fire TV (Prime Video), Nvidia Shield (Netflix, Prime Video), Android TV+[SmartTubeNext](https://github.com/yuliskov/SmartTubeNext) (Youtube)  

<!-- Sub-Section -->

### What refresh rate should I run on my HTPC?

Whatever refresh rate matches the framerate of the bulk of the content you play, if automatic [Refresh Rate Switching](/wiki/video#application-specific-setup-for-resolutionrefresh-rate-switching) is not available for your media players. If you use a 120 Hz display you can run at that instead of the refresh rate for the 23.976/24/30/60 frame rates below. If you're running 25/50 fps content, run at 50 or 100 Hz.  
Content varies between 23.976, 24, 25 fps, 29.97 or 60 fps. Local content is usually 23.976 fps (23 Hz) in North America and 25 fps (25 Hz) in Europe. Youtube is 24/25/30/60 fps. Netflix is 23.976/24/25/29.97 fps.  

<!-- Sub-Section -->

### Why does my HTPC change audio/display settings when switching inputs or waking from Sleep/Power up?

[See here](/wiki/audio#why-does-my-htpc-change-audiodisplay-settings-when-switching-inputs-or-waking-from-sleeppower-up)  

<!-- Sub-Section -->

### What is the best way to change DisplayPort/USB-C to HDMI. What are the limitations associated with doing this?

There are 2 ways to change DisplayPort to HDMI. The 1st is a Passive cable/adapter, the 2nd is an Active cable/adapter.  

A passive cable/adapter does not do a conversion on the protocol and is more limiting. If you have a DisplayPort 1.2 port, you can passively use HDMI 1.4 on the other end; so 4k@30 Hz SDR for video. Passive is most commonly used to get HD audio out of a DisplayPort port connected to a CPU's iGPU and send it to an AVR via HDMI on the other end.  

An active cable/adapter converts the DisplayPort protocol coming into the adapter. This is less limiting and will potentially provide higher bandwidth. For instance, you can use an Active adapter to convert DisplayPort 1.2 to HDMI 2.0 and get 4K@60Hz output, though getting some HDMI 2.0-native features is problematic if they weren't supported by the DisplayPort version to begin with. In our example, since DisplayPort 1.2 does not support HDR, it will not get passed over the adapter.  
SOME oem vendors (hp, dell, levovo) SOMETIMES advertise DisplayPort 1.2, but in reality support 1.3/1.4. When this happens you can use a DisplayPort 1.4->HDMI 2.0 active adapter and get HDR. This support is very spotty, so unless you find accounts of it on the hardware you want to use, don't bet on it.  

Active connectors can also be used to convert DisplayPort 1.4 to HDMI 2.1 and get 4K@120Hz HDR >= 32Gbps output. This also has its caveats. The adapters require the Display Stream Compression (DSC 1.2) feature to be supported in the GPU for use over DisplayPort. Since this is an OPTIONAL feature to DisplayPort 1.x, do not expect all GPUs with DisplayPort 1.4 to support this. Officially supported GPUS are >= Nvidia GTX 16xx/RTX 20xx or >= AMD RX 5xxx dGPUs.  
Active adapters also do not allow passthrough/bitstreaming of HD audio, only PCM audio.  

USB-C is just a different connector, still carrying the DisplayPort protocol as if it was that connector.  

When buying cables and adapters, please do NOT buy no-name brands. As quality control is low on them and marketing is more often than that mis-leading. Recommended cables and adapters can be found in the cables section of the [Hardware Components Guide](/wiki/components#video-cablesadapters). You can also find there what versions of DisplayPort and HDMI are supported on various CPUs/GPUs.  

<!-- Sub-Section -->

### What options are there for 4k @ 120 Hz video output?

Keep in mind we assume a HDMI input will be on your Display (TVs/Projectors, which is our only concern here).  

You will need to have HDMI 2.1 bandwidth on every HDMI device between your HTPC and your Display (GPU, TV, AVR, Switches, etc..). Simply having "HDMI 2.1" does not mean 4k@120 Hz bandwidth will be supported; this is an important distinction, so make sure they state 4k@120 hz support and/or >= 32 Gbps bandwidth (for at least media content) or >= 40 Gbps for gaming.  

**Options below for this are ordered from best to worst in terms of stability and reliability.** 

Technically, straight HDMI is the best (#1/#2/#3), followed by Thunderbolt->HDMI (#4/#5), USB-C->HDMI (#6) and DP->HDMI (#7/#8). 

Use case is KEY, as 4k@120 Hz is a broad requirement and knowing what sub-features (media, gaming, HDR) you want will determine bandwidth requirements. 

Use of an adapter in options #4/#5/#6/#7/#8 assumes you have a GPU with Displayport 1.4 protocol support and DSC (Display Stream Compression). 
Media content (HDR/10-bit/4:2:2) is technically possible without DSC support. Gaming (HDR/10-bit/4:4:4/RGB) is NOT. **VRR** gaming will **not** be supported with any adapter.  
  
1. DiY: Any [decent cpu/motherboard](/wiki/components#motherboards) or [OEM build](https://www.ebay.com/sch/i.html?_from=R40&_nkw=sff+%28i5-7400%2Ci3-8100%2Ci5-8400%2Ci5-8500%2Ci3-9100%2Ci5-9400%2Ci5-9500%29&_sacat=179&_odkw=sff+%28i3-9100%2Ci5-9400%2Ci5-9500%29&_osacat=179&LH_BIN=1&_sop=15) + a discrete GPU w/a 4k@120 Hz HDMI 2.1. e.g. RTX 3050 6GB LP, Radeon RX 6400 
2. DiY: An AMD Ryzen 8xxxG or Intel Core Ultra 2xx desktop CPU and respective motherboard that states 4k@120Hz HDMI 2.1. e.g. Ryzen 8500G + ASRock A620I/B650I Lightning Wifi mobo/ASRock Deskmini X600, Intel Core 225 + ASRock B860I Lightning, for a realistic max of 4:2:2 10-bit HDR. 
3. Pre-built: A Ryzen 6000+ or Intel 11th+ gen Mini PC with a 4k@120Hz HDMI 2.1 port. e,g. Ryzen: Minisforum UM760 Slim, Beelink SER6 Max, ASRock 4x4 7535U/8640U, Intel: Gigabyte Brix Extreme
4. Pre-built: An Intel 11th+ gen Mini PC with a Thunderbolt display out connector and a Thunderbolt->HDMI adapter/cable. e.g. Intel NUC [11](https://www.google.com/search?q=nuc11pahi5&oq=nuc11pahi5)/[12/13](https://www.newegg.com/p/pl?N=100008345%2050001157%20601331497&Order=1&SrchInDesc=nuc+12)/Lenovo IdeaCentre Mini Gen 8 + [Thunderbolt->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M) 
5. DiY: Intel 12th+ Gen CPU and respective motherboard with a Thunderbolt display out connector out and a [Thunderbolt->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M). Not as good as straight HDMI, but better compared to DP or plain USB-C. This will likely be expensive as these boards are rare. e.g. for an ITX board, look at the Asus ROG STRIX Z690-I GAMING WIFI, ASRock Z690 Phantom Gaming-ITX/TB4 or ASRock Z790 PG-ITX/TB4. 
6. Hybrid/DiY: An Intel 11th+ gen CPU and motherboard w/a USB-C Display Out and a USB-C->HDMI adapter/cable. e.g. ASRock Deskmini B660 + 
[USB-C->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M). 
7. DiY: Intel 12th+ Gen CPU and respective motherboard with a Displayport 1.4 connector and an Active DP->HDMI adapter. This tends to be the least stable option, so we don't recommend it at all.
8. Pre-Built: Ryzen 4000+ Mini PC with a Displayport 1.4 connector and an Active DP->HDMI adapter. e.g. Beelink SER5 5560U. This tends to be the least stable option, so we don't recommend it at all.
9. Headless Moonlight/Sunshine Streaming Host: [DP 1.4->HDMI 2.1 adapter](https://www.amazon.com/Cable-Matters-102101-BLK-Computer-Adapter/dp/B08XFSLWQF) + [VDD](https://github.com/itsmikethetech/Virtual-Display-Driver)/[IddSampleDriver](https://github.com/roshkins/IddSampleDriver) to create a virtual display. Alternatively, for a hardware solution use a [HDMI dummy plug](https://www.amazon.com/Headless-Display-Emulator-Generation-Single/dp/B07FB8GJ1Z) + Nvidia custom res/CRU res mod OR a [EDID Emulator](https://www.gofanco.com/prophecy-edid-emulator-pro-edidemul.html) to copy the host display's EDID.


<!-- Sub-Section -->

### How do I configure my app/gpu/display for proper color reproduction?

See above sections [Setup For Color Conversion/Reproduction](/wiki/video#setup-for-color-reproduction) and [Video Calibration Testing](/wiki/video#video-calibration-testing)  

<!-- Sub-Section -->

<!--
### How do I burn a digital video file to a physical disc?

DVD: Use DVD Flick to create and burn the disc from the source video file.  

Blu-Ray: Use tsMuxer or BD Rebuilder to create the Blu-Ray folder structure from the source video file. Use ImgBurn to burn the folder structure to the disc.  

-->

<!-- Sub-Section -->

### Where do I find additional sample video files to test?

These files must be downloaded for the media player(s) you are testing against. Do NOT play them in your browser.  

[AVS HD 709 Test Patterns](https://www.avsforum.com/threads/avs-hd-709-blu-ray-mp4-calibration.948496/) - Tests for basic video calibration  

Judder Tests - Tests for judder at varying frame rates - [23.976/24/25/29.97/30/50/59.94/60 fps](https://drive.google.com/uc?id=176bowvl5QMIw3TNbBFTaeax1aWf7WpG0) 

Frame Rate Tests - Tests for proper motion playback - [23.976 fps](https://drive.google.com/uc?export=download&id=1fmE-ois5fzwVlGccBf3HbBqjv5R_Etv5), [24 fps](https://drive.google.com/uc?export=download&id=1NWdrqmUHg4E_qMiSWoIp1AmV7Ulwm-zb), [25 fps](https://drive.google.com/uc?id=1UimhkIaljhhP3jbuHM75h7yk_WRwkxwQ), [29.97 fps](https://drive.google.com/uc?export=download&id=1K2khAth6dXg3Y1x3crKbaYrR7aRy3q_D)   

Audio Sync Tests - Tests for proper audio/video syncing - [1080p/H264/60fps/AAC](https://drive.google.com/uc?export=download&id=15ybDrQIZ1u4nkgEGlAaKMRhfuUuyj369), [1080p/HEVC/23.98fps/PCM](https://drive.google.com/uc?export=download&id=1xmIAh0YdM7asnUovRpCcxJeVdguOGxg7), [1080p/HEVC/24fps/PCM](https://drive.google.com/uc?export=download&id=1OaWTh3r6f7E9Ae8De57qFL9jGbsBeJni), [1080p/HEVC/29.97fps/PCM](https://drive.google.com/uc?export=download&id=11DG_qaM2xereJvxe2MedKqC3w7T3rgD9)  

<!--
[Jellyfish Video Bitrate Test Files](https://repo.jellyfin.org/test-videos/) - 1080p/4k, h.264/HEVC, 30 fps, High/Main (8-bit), Main10 (10-bit), MKV  
--> 
Jellyfish Codec Tests - Test if GPU can HW accelerate a codec - 1080p, 29.97 fps - [h.264](https://drive.google.com/uc?export=download&id=1z2bN5OH3Lc83ufEIv88zy4EDXOKfb6aa), [HEVC 8-bit](https://drive.google.com/uc?export=download&id=1W2luOdBL3XGOKif16vyWUHTouIDWyBBT), [HEVC 10-bit](https://drive.google.com/uc?export=download&id=1OD6C0wuauUhaDY3nGUeKt-e3IhLcwxXL), [HEVC 12-bit](https://drive.google.com/uc?export=download&id=1zyNr-xaneQrH-jXBhu9JxJXEL-t0aV4F), [AV1 8-bit](https://drive.google.com/uc?export=download&id=1G55AvJCbTrr29vkUDr7Qd1VaaYYwvpQS), [AV1 10-bit](https://drive.google.com/uc?export=download&id=19A4MaxBvdEkukV5fcDewfic4meXzPMPT), [VP9 8-bit](https://drive.google.com/uc?export=download&id=1RubNRLPNbg3mV7WE1RAJV6j4prAZsdXC), [VP9 10-bit](https://drive.google.com/uc?export=download&id=1oswygGTYOwjbxMG11oMSpQ8zZp2yRGDH), [MPEG2](https://drive.google.com/uc?export=download&id=1ngxW9r7oMyVdPo3OsoRQ-4lFUDgkzZ8m)  

<!--
[Jellyfin Video Bitrate Tests](https://repo.jellyfin.org/jellyfish/) - 1080p/4k, h.264/HEVC/**AV1**, 60 fps, High/Main (8-bit), Main10 (10-bit), HDR10/DV, MP4  
-->
[Jellyfin Video Bitrate Tests](https://repo.jellyfin.org/test-videos/) - Test if GPU can decode a video bitrate without dropping frames - 1080p/4k, h.264/HEVC/**AV1**, 60 fps, High/Main (8-bit), Main10 (10-bit), HDR10/DV, MP4  

Ideal Youtube tests - Test if GPU can decode youtube content - 1080p/4k, VP9/AV1, SDR/HDR, 60 fps, webm - [1080p](https://drive.google.com/uc?export=download&id=1xNV5Bq7a1nxEstoCm_A8Qbc0Ydeh0Xy4), [4K](https://drive.google.com/uc?export=download&id=1K0TrYoM5rn2dAkJ8-L9QGu6H0WNTQsR1)

[Ideal 4K HEVC test](https://drive.google.com/uc?export=download&id=1ZVwgFM7LEFTVE8KuNm_X7b1VfWcc-myN) - Test if GPU can decode a non-HDR high-end video file - UHD Blu-Ray max bitrate - 4k, HEVC, SDR, 120Mbps, 10-bit, 30 fps, mp4  

[Our HDR10 Test Videos/Patterns](https://drive.google.com/uc?export=download&id=1HbVqzhhtncjkowdxBgZ-ghycvy5w2cpv) - Tests for checking Basic HDR video calibration  

[Mehanik's Full HDR10 Test Videos/Patterns](https://drive.google.com/drive/folders/1m4IBq0euAxamL9ePgfdFuf8_5nLcRwHA) - Tests for checking Advanced HDR video calibration  

[Ideal 4K HEVC HDR10 test](https://drive.google.com/uc?export=download&id=1Q2Ix3mXMl-EMs0-hE-C3gCHg_Uwh4HZz) - Test if GPU can decode and process a HDR, high-end video file - UHD Blu-Ray high bitrate - 4k, HEVC, HDR10, 50-90Mbps, 10-bit, 29.97 fps, mp4  

[Other 4K Media Test Files](https://4kmedia.org) - 4k, h.264/HEVC, HDR10/DV, TS/MKV/MP4, 24-60 fps  

[Other Media Test Files](https://kodi.wiki/view/Samples) - 720p/1080p/4k, 23.976/24/25/29.97/59.94/60 fps, h.264/HEVC/AV1/VP9/MPEG2  

<!-- Section -->

## Accessories

**HDMI extenders**  

4k@60Hz + USB: [OREI](https://www.amazon.com/dp/B0BPVX4VYT)  

4k@60Hz + IR/Audio: [OREI](https://www.amazon.com/dp/B0BPW1ZC1B)  

4k@120Hz: [gofanco](https://www.gofanco.com/products/hdmi-extenders/hdmi-extenders-over-ethernet/hdmi-cat-extender-4k120-40m-hdext4k120.html)  

**HDMI Splitters**  

4k@120Hz: [Monoprice Blackbird](https://www.monoprice.com/product?p_id=44436)

**HDMI EDID Emulators**  

[Prophecy EDID Tester](https://www.gofanco.com/prophecy-edid-emulator-pro-edidemul.html)


<!-- Footer -->
&nbsp;

---

*This page was last updated on 2025-04-18*

