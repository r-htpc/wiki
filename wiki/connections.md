---
description: Information on the best ways to connect your HTPC to a sound system and/or HT display.
---

# Connection Setup Guide

**This page is best viewed with a PC web browser.**  

<!-- Section -->

## **Setup**

<!-- Sub-Section -->

### **Introduction**  

For simplicity, the term “HTPC” used here can mean either a PC or a streaming device, like a Roku/Fire TV/etc, except where differences are noted. 
The term “Sound System” can mean an AV Receiver, Amplifier, Soundbar, DAC, Speakers or Headphones. The term “Display” can mean a TV or Projector.

There are many ways to connect your HTPC/media device to your Sound System and HT Display.  
This could be with HDMI, DisplayPort, Optical/SPDIF, RCA, 3.5mm or a combination of any of them.  
This is a complicated topic given that you probably have at least 3 pieces of hardware (HTPC, Sound System, Display) that have various connection 
types/capabilities and have to agree on what they will do together. As such this wiki page can be overwhelming and get confusing quickly, 
so read this page carefully and multiple times if you have to. 

**Understanding Audio and Video technologies (formats, codecs, interfaces, etc..) is very useful before continuing. If you're unfamiliar with them, 
you are urged to read the Technologies section of the [AUDIO Setup Guide](/wiki/audio#technologies) and [VIDEO Setup Guide](/wiki/video#technologies) first.**

Before you try any of the following scenarios, consider what you're trying to achieve and what your hardware is capable of; What resolutions and 
refresh rates are you trying to display? What audio codecs are you trying to play? Are you gaming and is VRR (g-sync/freesync) required? What ports are 
on your sound system and display and what specs are they (HDMI 1.x/2.x, DisplayPort 1.x/2.x, optical, rca), etc.. This information is critical 
and should be gotten from your device manuals and spec pages on the mfgr's websites. Armed with those and with the information in Technologies sections referenced 
above, you should have a good idea of what your hardware is capable of and a good sense of the optimal scenario for what you're trying to achieve. 
If you ask us for help, provide all this information, so we can better help you. 

<!-- Sub-Section -->

### **Hardware Setup**  

Scenarios are listed as Most Desirable to Least Desirable.  

Scenario #1 listed below, with video passthrough through your sound system, is the best scenario. However, if you have an older sound system that doesn't support video passthrough for the features you need, like 4k, HDR or high refresh rates for gaming, then the best scenarios in order are: #2 (earc), #3, #4, #2 (arc/optical).  

Consult [this section](/wiki/components#video-cablesadapters) of the Hardware Components Guide for cable/adapter recommendations. Consult [this section](/wiki/audio#what-kind-of-sound-system-should-i-get) below for sound system recommendations.  

**Scenario #1** - The ideal scenario, connecting your HTPC to your sound system and then your sound system to your TV

<img src="https://i.imgur.com/MWYvscz.png" width="550" height="300" alt="DIAGRAM">

<!-- ![DIAGRAM](/assets/images/audio-diagram-1.png) -->

In this scenario, the sound system gets the audio and video first and then passes the video through to the display, e.g. HTPC (HDMI) -> Sound System (HDMI) in -> Sound System (HDMI) out -> TV (HDMI).  
When the sound system supports the required video resolution for passthrough to the display, this scenario is simple and provides the highest compatibility and best audio support.  

1. Connect the HTPC's primary HDMI output to the Sound System's HDMI input, e.g. HTPC (HDMI) -> Sound System (HDMI). If you only have a Displayport/USB-C connector, use an ACTIVE [adapter](/wiki/components#video-cablesadapters) first, but expect to be limited to Lossy codec/PCM audio. Otherwise, see Scenario #3.
2. Connect the Sound System's HDMI output to an HDMI input on the Display.
3. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

Where this doesn't work is when the sound system:  

1. Doesn't support the required video resolution/refresh rate for passthrough to the display. e.g. you want to pass through 4k video to a 4k tv but the sound system only supports 1080p passthrough. See alternate scenarios below.  
2. Doesn't have both input and output hdmi ports (e.g. cheap soundbars with only 1 HDMI ARC port) or no HDMI ports (only S/PDIF/Optical). See alternate scenarios below.  

**Scenario #2** - Your display & sound system have a HDMI (e)ARC or Optical port

<a href="https://i.imgur.com/3HpEIni.png"><img src="https://i.imgur.com/3HpEIni.png" width="550" height="300" alt="DIAGRAM"></a>

This will send audio through your display. This is common for VRR (gsync/freesync) gaming setups and/or where the desired resolution/refresh rate to the display exceeds what the sound system can pass through.  

1. Connect the HTPC's HDMI output to the display's HDMI non-(e)ARC input, i.e. HTPC (HDMI) -> TV (HDMI).  
2. Connect the display's HDMI (e)ARC/Optical output to the sound system's HDMI (e)ARC/Optical input, i.e. TV (e)ARC (HDMI/Optical) -> Sound System (e)ARC (HDMI/Optical).  
3. Change the settings in the sound/audio output, CEC sections of your display's interface.
   - Enable HDMI CEC
   - Enable pass-through/bitstream digital audio.
   - Roku has a [good guide](https://support.roku.com/article/360034303013) for many display mfgrs
4. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

 Video supported: Negotiated by HTPC and Display  

 Audio supported: Stereo PCM, Lossy DD+ 5.1/DTS 5.1 (ARC) or All (eARC) - Dependent on your display's audio pass-through support. See your display's manual or [rtings.com](https://rtings.com/tv) reviews for what audio codecs are supported and how to configure your display to pass-through/bitstream audio. If your display can't pass-through the codecs you want, see below scenarios. **If your display supports eARC but your sound system doesn't**, use an [eARC extractor](https://www.amazon.com/ViewHD-Adapter-Audio-Receiver-Application/dp/B08ZHCS5D9) between the display and the sound system's HDMI **input**.  

**Scenario #3** - Your HTPC has/[could have](/wiki/components#gpusgraphics) multiple display outputs (hdmi/displayport/usb-c display out)

<img src="https://i.imgur.com/mrtX8DH.png" width="550" height="300" alt="DIAGRAM">

This will give you a primary display for video output and a secondary, extended display for audio-only output. This is common for VRR (gsync/freesync) gaming setups and/or where the resolution/refresh rate to the display exceeds what the sound system can pass through. If a secondary display is not desirable, see Scenario #4.  

1. Connect the HTPC's primary HDMI output to the display's HDMI input, e.g. HTPC (HDMI) -> TV (HDMI).  
2. Connect the HTPC's 2nd display output (either from motherboard or dGPU) to the sound system. If Displayport, use a PASSIVE [Displayport->HDMI cable](/wiki/components#video-cablesadapters) or adapter. e.g. HTPC (HDMI/Displayport) -> Sound System (HDMI).  
3. Set the 2nd display output in your OS as an extended display at a resolution of 720p@60Hz. Drag this display to the top-right corner of the primary display. NOTE: Even though you are using this only for audio, a video signal IS required.  
4. In Windows sound control panel, disable the audio device on the primary display output. Enable audio on the 2nd display output.  
5. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)
6. OPTIONAL: Use window management software to lock window placement to your primary display ([DisplayFusion](https://www.displayfusion.com/)/[MonitorSwitcher](https://sourceforge.net/projects/monitorswitcher/)).

 Video supported: Negotiated by HTPC and Display. DRMed content may not work properly if both display outputs are coming from the same GPU.  

 Audio supported: All  

**Scenario #4** - Your HTPC does/does not have multiple display outputs (either hdmi or displayport), you want full audio support, but you don't want to set up a cloned or extended display in windows for separate video/audio

<img src="https://i.imgur.com/f2qsP4W.png" width="550" height="300" alt="DIAGRAM">

This is an alternative to Scenario #3 where you don't want to deal with multiple displays in windows either out of navigational or visual annoyance due to driving multiple display outputs. It could also be used with a single display output (e.g. APU) where you want full audio support but don't have eARC on your display. If you have only an ARC/eARC port on your sound system (like a cheaper soundbar), use a [HDMI Splitter](/wiki/audio#accessories) with an eARC output.  

You will use an HDMI splitter to split/clone the source signal and send the same signal to both your display and sound system. Note that not all splitters are built the same and can vary dramatically in price, depending on feature set and reliability. See the [accessories](/wiki/audio#accessories) section.  

1. Connect the HTPC's primary HDMI output to a [HDMI Splitter](/wiki/audio#accessories).
2. Connect the 1st output of the HDMI Splitter to your Display.  
3. Connect the 2nd output of the HDMI Splitter to your Sound system.  
4. Set the dip switches on the HDMI Splitter to the desired behavior for display/edid priority.  
5. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

 Video supported: Negotiated by HTPC and Splitter, set by dip switches.  

 Audio supported: All  

 NOTES: DRMed content may not work due to old HDCP support on splitters. CEC may not work. HDMI 2.1 splitters are rare and/or expensive. Displayport splitters have a limit of 4K@60Hz on the primary conn. when using audio on the secondary conn.  

**Scenario #5** - Your HTPC does NOT have multiple display outputs, but does have an Optical/S/PDIF/3.5mm ports

<img src="https://i.imgur.com/dnBBvX3.png" width="550" height="300" alt="DIAGRAM">

In this scenario you will likely be bitstreaming through Optical, or in the case of 3.5mm jacks, decoding audio on the HTPC  

1. Connect the HTPC's primary HDMI output to the display's HDMI input, i.e. HTPC (HDMI) -> TV (HDMI).  
2. Connect the HTPC's optical/3.5mm output to the sound system's optical/RCA/3.5mm.. input, e.g. HTPC (Optical) -> Sound System (Optical).  
3. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

 Video supported: Negotiated by HTPC and Display  

 Audio supported: Stereo PCM, Lossy DD 5.1/DTS 5.1 (optical) or Stereo/Surround analog (3.5mm). [Gaming audio setup](/wiki/audio#how-do-i-configure-my-htpc-to-output-sound-for-games-to-my-sound-system)  

**Scenario #6** - Your HTPC does NOT have multiple display outputs, does not have an Optical/SPDIF port, and your display does not have a HDMI ARC or Optical port

<img src="https://i.imgur.com/vpUWS5B.png" width="550" height="300" alt="DIAGRAM">

If you have only an ARC/eARC port on your sound system (like a cheaper soundbar), use a [HDMI Extractor](/wiki/audio#accessories) with an eARC output.
 
1. Connect the HTPC's HDMI output to a [HDMI Audio Extractor](/wiki/audio#accessories)'s HDMI input, i.e. HTPC (HDMI) -> Audio Extractor (HDMI).  
2. Connect the HDMI Audio Extractor's HDMI output to the display's HDMI input, i.e. Audio Extractor (HDMI) -> TV (HDMI).  
3. Connect the HDMI Audio Extractor's HDMI audio/Optical/RCA/3.5mm ports to the sound system's HDMI/Optical/RCA/3.5mm ports.  
4. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

 Video supported: Negotiated by HTPC, Display and HDMI Audio Extractor  

 Audio supported: HDMI (all), Stereo PCM, Lossy DD 5.1/DTS 5.1 (optical), Stereo PCM (RCA), or Stereo/Surround analog (3.5mm). [Gaming audio setup](/wiki/audio#how-do-i-configure-my-htpc-to-output-sound-for-games-to-my-sound-system)  

 NOTE: An audio extractor will not DECODE audio codecs, it just passes it through its output connector. If you send such a bitstreamed signal into it and expect audio out of its analog connectors, you will get NO audio; you either have to pass PCM in to get audio out of those connectors, or use an AVR/decoder box behind the HDMI/optical port.  

**Scenario #7** - Your HTPC does have multiple display outputs (either hdmi or displayport) but your sound system does NOT have a HDMI port

<img src="https://i.imgur.com/jl7rIf7.png" width="550" height="300" alt="DIAGRAM">

1. Connect the HTPC's primary HDMI output to the display's HDMI input, i.e. HTPC (HDMI) -> TV (HDMI).  
2. Connect the HTPC's 2nd display output (either from motherboard or dGPU) to a [HDMI Audio Extractor](https://www.amazon.com/OREI-HDA-912-Audio-Converter-Extractor/dp/B07BHYXVTY)'s HDMI input. If Displayport, use a PASSIVE [Displayport->HDMI cable](/wiki/components#video-cablesadapters) or adapter. e.g. HTPC (HDMI/Displayport) -> Audio Extractor (HDMI).  
3. Connect the HDMI Audio Extractor's Optical/RCA/3.5mm ports to the sound system's Optical/RCA/3.5mm ports, i.e. Audio Extractor (Optical/RCA/3.5mm) -> Sound System (Optical/RCA/3.5mm).  
4. Connect a [HDMI dummy plug](https://www.amazon.com/Headless-Display-Emulator-Generation-Single/dp/B07FB8GJ1Z) to the HDMI Audio Extractor's HDMI Out port.  
5. Set the 2nd display output in your OS as an extended display at a resolution of 720p@60Hz. Drag this display to the top-right corner of the primary display.. NOTE: Even though you are using this only for audio, a video signal IS required.  
6. In Windows sound control panel, disable the audio device on the primary display output. Enable audio on the 2nd display output.  
7. Configure your media players for the audio codecs you can support per [Software/OS Setup](/wiki/audio#softwareos-setup)  

 Video supported: Negotiated by HTPC and Display  

 Audio supported: Stereo PCM, Lossy DD 5.1/DTS 5.1 (optical), Stereo PCM (RCA), or Stereo/Surround analog (3.5mm). [Gaming audio setup](/wiki/audio#how-do-i-configure-my-htpc-to-output-sound-for-games-to-my-sound-system)  

 NOTE: An audio extractor will not DECODE Dolby/DTS audio, it just passes it through to the optical connector. If you send such a signal in and expect audio out of the RCA/3.5" connectors, you will get NO audio; you either have to pass PCM in to get audio out of those connectors, or use an AVR/decoder box behind the optical port, like [this](https://www.amazon.com/J-Tech-Digital-Optical-Toslink-Converter/dp/B01A1HQE38).  

<!-- Sub-Section -->

### **Software Setup**  

Continue your setup by following the instructions in the [VIDEO setup guide](/wiki/video#setup) and [AUDIO setup guide](/wiki/video#setup).

<!-- Section -->

## Accessories

[Video accessories](/wiki/video#accessories)
[Audio accessories](/wiki/audio#accessories)  

<!-- Sub-Section -->

<!-- Footer -->
&nbsp;

---

 *This page was last updated on 2025-07-05*

