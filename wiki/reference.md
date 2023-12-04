# HTPC Term Reference

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

This is a list of terms you may find on this subreddit and what they mean

---

**4K** - See: UHD

**AAC/HE-AAC** - Multi-channel audio codecs. Part of the MPEG-2/MPEG-4 specs. Competitor to Dolby and DTS. Successor to MP3

**AC-3** - Synonymous with Dolby DD

**APU** - Accelerated Processing Unit. The term AMD gives to their CPU packages that have a GPU built-in. Common ones are Ryzen 2x00G-5x00G/7xxx (med. perf/power), Athlon 2x0GE/3000G (low perf/power), A4/A6/A8/A10/A12 (last gen), Athlon 5xxx (old).

**ARC/eARC (audio)** - Audio Return Channel. A feature in the HDMI spec that allows audio to flow from a HDMI sink (e.g. TV) back to a sound system. This is useful when an HTPC/media device is connected to a TV first which then has to passthrough the HTPC audio (or its own audio) back to the sound system. ARC (HDMI 1.4/2.0) supports 2.0 PCM uncompressed and DD 5.1/DTS 5.1 compressed audio. eARC (HDMI 2.1) support up to Dolby Atmos/DTS:X uncompressed audio. ARC almost never supported on HTPC/media device GPU ports, only on Displays and sound systems.

**ARC (Intel)** - Family of dedicated video cards made by Intel. Supports DP 1.4a/2.0, HDMI 2.0b/2.1, 4k netflix, AV1 decoding/encoding.

**AV1** - An open, royalty-free video codec. Lossy compression. The successor to and 20-40% more efficient than VP9/HEVC. Not widely used as of 2021; found in some Youtube/Netflix content. Supported by Intel >= 11xxG/11xxx, >= Arc 3, Nvidia >= RTX 30-series, AMD >= RX 66xx, >= Ryzen 6xxxU, >= Ryzen 7xxx.  

**AVC** - A video codec synonymous with H.264/mpeg-4.

**AVR** - Audio/Video Receiver. A piece of hardware that receives multiple audio/video input signals (from a HTPC/Blu-ray player/Video game console/etc..), amplifies audio, applies audio processing, delivers audio to speakers and video to output devices such as TVs.

**<name> Lake** - A modern generation of Intel CPU

ARCH|GEN|RELEASED|NOTES
:--|:--|:--|:--
[Skylake](https://en.wikipedia.org/wiki/Skylake_\(microarchitecture\))|6th Gen|Mid-2015|Hybrid-based HEVC decoding. SGX. 1xx/2xx series chipset.
[Kaby Lake](https://en.wikipedia.org/wiki/Kaby_Lake)|7th Gen|Late-2016|Hardware HEVC decoding. DRM for 4k netflix/UHD Blu-Ray. 1xx/2xx chipset.
[Coffee Lake](https://en.wikipedia.org/wiki/Coffee_Lake)|8/9th Gen|Mid-2017/8|2-8 core CPUs. Removal of DDR3 support. 3xx series chipset ONLY
[Comet Lake](https://en.wikipedia.org/wiki/Comet_Lake)|10th Gen|Mid-2020|2-10 core CPUs. DDR4-2933 memory support. 4xx series chipset ONLY
[Rocket Lake](https://en.wikipedia.org/wiki/Rocket_Lake)|11th Gen|Mid-2021|2-8 core CPUs. DDR4-3200 memory support. 4xx/5xx series chipset. Introduced HDMI 2.0/DP 1.4 native on an Intel desktop CPU (>= i5). AV1 decoding. Removed SGX support.
[Alder Lake](https://en.wikipedia.org/wiki/Alder_Lake_\(microprocessor\))|12th Gen|Late-2021|2-16 core CPUs. DDR4-3200/DDR5-4800 memory support. 6xx/7xx series chipset. HDMI 2.0/DP 1.4 on all CPUs.
[Raptor Lake](https://en.wikipedia.org/wiki/Raptor_Lake)|13/14th Gen|Late-2022/3|14-24 core CPUs. DDR4-3200/DDR5-6000 memory support. 6xx/7xx series chipset. HDMI 2.0/DP 1.4 on all CPUs.
[Apollo Lake](https://en.wikipedia.org/wiki/Goldmont)|7th Gen|Mid-2016|Technically under the Goldmont arch, but similar to Kaby Lake in a smaller form factor/feature set/power usage profile.
[Gemini Lake](https://en.wikipedia.org/wiki/Goldmont_Plus)|8th Gen|Early-2018|Technically under the Goldmont Plus arch, but similar to Coffee Lake in a smaller form factor/feature set/power usage profile. Introduced HDMI 2.0 native on CPU.

**CEC** - Consumer Electronics Control. A technology used to allow devices to control other devices over a HDMI cable. e.g. when you turn on your AVR, a CEC signal can turn on your TV. CEC is only built-in to a limited amount of PCs, like 6th gen NUCs and up, for power-on capability. You can add USB-CEC adapters for support on other PCs.

**Dolby DD/DD+/TrueHD/Atmos** - Multi-channel audio codecs. Competitor to DTS.

**DTS/DTS-HD/DTS-HD MA/DTS:X** - Multi-channel audio codecs. Competitor to Dolby.

**DRM** - Digital Rights Management. A suite of access control technologies used to protect content from unauthorized content duplication. HDCP is a form of this.

**DisplayPort/DP** - An interface for transporting audio/video. Commonly used to connect devices in a Home Theater setting, but not nearly as common as HDMI. As TVs and AVRs tend to have HDMI ports, DisplayPorts that are found on HTPCs are usually used in conjunction with a DisplayPort->HDMI adapter when a HDMI 2.0 port is not found on the motherboard to get HDMI 2.0 output. The current standard is DisplayPort 1.4

**E-AC-3** - Synonymous with Dolby DD+

**FPS** - Frames Per Second. This is used for video output in reference to how many content frames are recorded/shown/transmitted per second. A higher number usually translates to smoother video.

The gold standard today in HTPCs is 4k@60FPS. Common rates relating to HTPCs are:

RATE|USE|NOTES
:--|:--|:--
23.976/24|Movies|Usually upconverted to 60i for TVs through a process known as 2:3/3:2 pulldown.
25|Broadcast TV (outside US/Central America/SE Asia)|Standard used in PAL color-encoding for 576i
29.97/30|Broadcast TV (US/Central America/SE Asia), HTPC|Standard used in NTSC color-encoding. Interlaced to 60 fps for TV
60|HTPC and TV Display|60i (cable/sat), 60p (HTPC, media devices)

**Form Factor** - An aspect of hardware design typically relating to the size and shape of components. Commonly used in HTPCs for cases and motherboards.

NAME|SIZE (in)|SIZE (mm)|NOTES
:--|:--|:--|:--
pico-ITX|3.9 x 2.8|100 x 72|
NUC|4 x 4|101.6 x 101.6|
nano-ITX|4.7 x 4.7|120 x 120|
mini-ITX|6.7 x 6.7|170 x 170|PCIE x 1, MEM x 2
thin-ITX|6.7 x 6.7|170 x 170|mini-ITX w/25mm vs 44mm shield. SODIMM RAM instead of UDIMM
micro-ATX/uATX/M-ATX|9.6 × 9.6|244 × 244|PCIE x 3/4, MEM x 2/4
ATX|12 x 9.6|305 x 244|PCIE x 5/6, MEM x 2/4

**GPU/iGPU** - Graphics Processing Unit. A video card. The 'i' in iGPU stands for 'Internal/Integrated'. This is a GPU that is included on the CPU package, prevelant in Intel CPUs (HD xxx) and AMD APUs (Radeon/Vega).

**GTX/RTX 10xx/16xx/20xx/30xx/40xx** - Families of high-end graphics cards made by Nvidia. There are various versions, 1030/1050/1060/1070/1080 ($75-$500), 1650/1660 ($150-$250), 2060/2070/2080 ($350-$1200), 3070/3080 ($500-$700). They are currently one of the only graphics card families to support HDMI 2.0, HDCP 2.2 and Microsoft Playready 3 (outside of Intel iGPUs >= 7th gen, AMD APUs >= 3200G and AMD dGPUs >= RX 4xx) for DRM use to access 4K Netflix. RTX 30xx adds support for HDMI 2.1

**H.264** - A video codec. Also called AVC. Lossy compression. Used by Netflix, Hulu, Amazon Prime, Vimeo, Youtube, iTunes and various HDTV broadcasts. Used in blu-ray discs. Widely supported since the early 2010s.

**H.265/HEVC** - A video codec that is the successor to H.264. Lossy compression. Better quality for same bitrate. Used by Netflix. Used in UHD blu-ray discs. Supported by >= Intel Kaby/Apollo Lake, >= Intel ARC 3, AMD Ryzen APUs/dGPUs >= RX 4xx, >= Nvidia GTX 10-series

**HDCP** - High-bandwidth Digital Content Protection. A copy-protection/DRM scheme found in audio/video streams to protect content from unauthorized duplication. Commonly found in DVD, Blu-ray, Netflix and other major streaming content and used over HDMI, DisplayPort and DVI video interfaces. Each hardware device (HTPC, AVR, TV, etc..) in the content chain must be HDCP compliant for the stream to be accessible. For a HTPC, this usually means the CPU, GPU, video interface, OS and ultimately your output device (typically a TV). The current standard is HDCP 2.2.

**HDMI** - High-Definition Multimedia Interface. An interface for transporting audio/video. Commonly used to connect devices in a Home Theater setting. The current standard is HDMI 2.1.

**HDR video** - High Dynamic Range video. A technology used to produce better looking video by preserving details in the darkest and lightest portions of a frame resulting in better contrast. For a HTPC, this means HDR support must be in the video, GPU, video interface (HDMI/DP) and ultimately your output device (typically a TV). Check the [FAQ](/htpc-wiki/faq#wiki_what_is_hdr_video_and_what_do_i_need_to_take_advantage_of_it.3F) for GPUs that support HDR. Common standards are HDR10, HDR10+ and Dolby Vision.

**HTPC** - Home Theater Personal Computer. Why you are here!

**Hz** - Hertz. Commonly referred to as Refresh Rate. Ideally Hz >= FPS. It's still common for Refresh Rate to be multiple times the FPS. For instance, you can have 60 Hz and 30 FPS in which the output device will display each frame twice. This is most commonly used for video output and a higher number means less video flicker and higher image stability.

The gold standard today in HTPCs for media is 60 Hz. For high end gaming, 120 Hz is desirable, but uncommon as of yet. Common rates relating to HTPCs are:

RATE|USE|NOTES
:--|:--|:--
24|NTSC|For judder reduction of 24p content (movies, almost all 1080p bluray)
30|NTSC|Older TVs use this. For 30fps
50|PAL|For 25fps
60|NTSC|Majority of TVs use this. Used for 60fps
120|NA|Used in high-end TVs for better motion because 24fps movies evenly multiplies to 120 therefore does not need 2:3 pulldown
240|NA|Used to simulate even better motion by rapidly turning the TV backlight off and on at an additional 120 Hz

**Judder** - A common display artifact caused by playing 24p content on a display with a refresh rate (typically 60hz) that doesn't equally divide by the frame rate. This causes stuttering in horizontal motion and panning scenes as the display uses a method called 'pulldown' to fit the frames into the refresh rate. Typical workarounds are switching the display into 24Hz mode or using a display with a true refresh rate that divides equally (such as 120Hz).

**madVR** - A DirectShow video renderer usually added to video players (like kodi, mpc-hc, etc..) to enhance video content using GPU computing power. This includes, but is not limited to, passthrough and processing/tonemapping of HDR metadata for displays, HQ image upscaling/downscaling, chroma upscaling, artifact removal, image enhancement, smooth motion, dithering and deinterlacing.

**MP3** - A multi-channel audio codec. Generally stereo up to 320Kbps. Succeeded by AAC.

**NAS** - Network Attached Storage. A device that holds 1 or more disks connected to a network for serving media to clients over said network. For HTPC use, an example would be a NAS with 4 disks in a RAID 5 configuration. Media would be shared using a file share, which is accessed by something like Plex Media Server or a Kodi client. Fully featured NASes also have the ability to run media services on them like a media server, media grabbing software, VPN, etc..

**NTSC** - National Television System Committee. Television color-encoding for 480i. 60hz. Usually used in the US/Central America and northern parts of South America.

**NUC** - Next Unit of Computing. A 4x4 form factor for PCs, developed by Intel. Also used to reference an actual PC of this form factor. They usually have an external power supply, a VESA mount and simply require you to add memory and storage for a complete system.

**OTA** - Over the Air. Terrestrial services (usually TV) via RF Antennas. Analog until 2009. 

**PAL** - Phase Alternating Line. Television Color-encoding for 576i. 50 Hz, 25fps. Usually used outside US/Central America and northern parts of South America.

**RAID** - Redundant Array of Inexpensive Disks. A technology used in media storage to provide scale-ability or redundancy/resiliency against loss of data due to storage medium (typically disks) failure. Typically found on storage in NAS devices and internal storage on high-end HTPCs. Popular forms are RAID 0 (for scale-ability), RAID 1 (for redundancy), RAID 5 (for scale-ability+redundancy).

**Raven Ridge/Picasso/Renoir/Cezanne** - AMD's 2xxx/3xxx/4xxx/5xxx series of "G" APUs based on their Zen architecture (2017-). These integrate a GPU into the CPU package.

**RTX** - See GTX

**RX 4xx/5xx** - Older generation family of mid-level graphics cards made by AMD. It is one of the graphics card families to support HDMI 2.0, HDCP 2.2 and Microsoft Playready 3 for DRM use to access 4K Netflix.

**RX Vega/Navi/5xxx/6xxx/7xxx** - Families of graphics cards made by AMD. Vega (2017-) is found in AMD APUs in various forms, supporting HDMI 2.0 and HDR. Also found in dedicated GPUs in the form of Vega 56/64, succeeding the RX 4xx/5xx families. Navi (2019) succeeds Vega with RDNA 1 and includes the RX 5x00 dedicated GPUs. Navi is one of the graphics card families to support HDMI 2.0, HDCP 2.2 and Microsoft Playready 3 for DRM use to access 4K Netflix. RDNA 2 include RX 6xx0 dedicated GPUs and Ryzen 7xxx iGPUs, and adds support for HDMI 2.1. RDNA 3 include RX 7x00 dedicated GPUs and adds support for DP 2.1.

**Ryzen/Zen** -  A modern generation of AMD CPU

ARCH|GEN|RELEASED|NOTES
:--|:--|:--|:--
[Zen](https://en.wikipedia.org/wiki/Zen_\(microarchitecture\))|1st Gen|2017|AM4 14nm. 1xxx-series CPUs. 2xxx-series APUs. A320/B350/B450/X370/X470 series chipsets.
[Zen+](https://en.wikipedia.org/wiki/Zen%2B)|2nd Gen|2018|AM4 12nm. 2xxx-series CPUs. 3xxx-series APUs. 4-8 cores. A320/B350/B450/X370/X470 series chipsets.
[Zen 2](https://en.wikipedia.org/wiki/Zen_2)|3rd Gen|2019|AM4 7nm. 3xxx-series CPUs. 4xxx-series APUs (OEM). 4-16 cores. X570/B550/A520 series chipsets. PCIe 4 support.
[Zen 3](https://en.wikipedia.org/wiki/Zen_3)|4th Gen|2020|AM4 7nm+. 5xxx-series CPUs. 5xxx-series APUs. 4-16 cores.
[Zen 4](https://en.wikipedia.org/wiki/Zen_4)|5th Gen|2022|AM5 5nm. 7xxx-series CPUs. 6-16 cores. X670/B650 chipsets. PCIe 5, DDR5, built-in RDNA 2 iGPU.

**SFF** - Small Form Factor. A computer case form factor for desktop computers optimized for space (smaller than a Mini Tower), so ideal for HTPC use. It usually is short and tends to have 1x3.5" internal drive bay and, at most, have 1x5.25" drive slot. It can be various sizes buy usually it's around 14"x13"x4" (WxDxH) and a mean of 14 liters.

**SGX** - Software Guard Extensions. Used for implementing DRM to allow UHD blu-ray disc playing on Intel platforms. Implemented in software and BIOS.

**TDP** - Thermal Design Power. The maximum amount of heat generated by a CPU. Usually used to determine power usage of a CPU in a system. For a HTPC, users try to use CPUs with a TDP of <= 65W. Capable CPUs may go all the way down to 4.5W-6W, depending on your needs.

**Tonemapping** - Technique used to map one set of colors to another. Commonly used to map HDR to SDR for displays that do not support HDR. madVR can be used for this. 

**UHD** - Ultra High Definition. A term used to refer to >= 4K resolutions supported by various display and rendering devices. The most common of these is 4K (3840x2160), which is twice the dimension size (or 4x the pixels) of FHD (1920x1080).

**VP9** - A video codec widely used on Youtube. Succeeded by AV1. Supported by >= Intel Kaby/Apollo Lake, AMD Ryzen APUs/dGPUs >= RX 5xxx, >= Nvidia GTX 10-series
