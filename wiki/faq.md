# Frequently Asked Questions

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

*This page is best viewed with a PC web browser.*  

If you're new to HTPCs, you should work your way through this page before moving on to other, more specific pages in our Wiki.  

<!-- Section -->

## What is a HTPC?

HTPC stands for Home Theater Personal Computer.

Traditionally a HTPC is a PC with a purpose to play and/or serve media in a theater-type setting (living room, etc..). It does this through specific hardware and/or software. 

Specific hardware can be a TV tuner card, high-end sound card, other decoder cards, remotes or a case optimized for noise and/or space.

[Specific software can be media players, codecs, certain operating systems and specialized media software interfaces](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up).

Media can be video content from [ripped personal discs](/wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use), [streaming services](/wiki/faq#can-i-use-my-htpc-for-streaming-from-services-such-as-netflix-youtube-amazon-hulu-etc), audio, photos, or emulation gaming content. If you are planning on playing streaming services in >= 1080p, or >= 5.1 sound, you should use a [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead. A traditional HTPC [lacks HD video/audio for a lot of the streaming services](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) and is poor at navigating them.

As computing power has gotten smaller and smaller, traditional PCs have given way to integrated media devices which have blurred the line over what a PC is.

A media device such as a Roku player is very small and performs most of the functions a PC does, with CPU, memory, storage, operating system, etc.. The biggest distinction is that [these devices](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) are usually designed specifically for playing streaming media in a Home Theater setting. 

MOST of these small devices simply act as clients; to internet streaming services, like Netflix and/or personal content you have on local or network storage. 

An example would be the Nvidia Shield TV. It is a powerful integrated device that's remote-oriented, with an Android media interface, supporting a wide range of streaming services, HDR and HD audio and video codecs for local content. It also can have storage connected to it which makes it a good all-in-one device.

**This can be confusing**; it's not a traditional HTPC per-se, but performs the functions of one. Both traditional HTPCs and media devices have their place. Each is better at different things. Media devices are better as a front-end, as things like ease of navigation and streaming service video/audio support is king. A traditional HTPC is better at being flexible; running wide-ranging programs and utility, high-end gaming, web browsing, doing high-end video and audio processing or transcoding, and the ability to be a server and holds large amounts of storage. For more arguments for/against, read our [section](/wiki/faq#why-would-i-use-a-pc-over-a-media-device-roku-firetv-shield-etc-for-a-htpc) below. 

Below we'll advise you on how to get started with a HTPC.

What is NOT a HTPC: Playing media just on your laptop. Playing media at your desk. Playing media on a computer monitor(s).

<!-- Section -->

## How do I get started with a HTPC setup?

A HTPC whether it be a PC or media device, can act as a client, a server, both or standalone.  

For instance, it can act standalone and play media from [internal storage](/wiki/storage) or [streaming services](/wiki/faq#can-i-use-my-htpc-for-streaming-from-services-such-as-netflix-youtube-amazon-hulu-etc) to a connected TV/sound system.
 - If you are planning on playing streaming services in >= 1080p, or >= 5.1 sound, you should use a [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead. A traditional HTPC [lacks HD video/audio for a lot of the streaming services](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) and is poor at navigating them.  
 - If you are planning on playing **Dolby Vision**/HDR10+, you should use a [media device](/wiki/sample-builds#specialized-dolby-vision--hdr10) instead. A traditional HTPC lacks proper passthrough of Dolby Vision for media content.
 
It can be a client connected to a TV/sound system and then [connect to a server](/wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device) which provides it the media/games to play.  
It can be a server which provides the media/games to the client as fore-mentioned.  
It can be client and server as well; connected to a TV as a client, playing internal media, but also has [server software](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) installed, which it uses to [send media to other clients in the home](/wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device).

You should first decide which of these roles you need and what your use-case is, then you can look at the builds page and find something that meets your needs.
 - If a client/standlone, decide what kind of content you want to play. Local content? What video codecs? What audio codecs? HDR? Streaming services? Which ones? Web browsing? Gaming? Budget? Size?
 - If a server, decide what content you want to serve. Will you have to transcode it for remote clients? Do you want internal storage for it? How much? Budget? Size?

If you're not familiar with HTPC terminology, you should reference the [video](/wiki/video), [audio](/wiki/audio), and [HTPC terms](/wiki/reference) pages of the wiki as a guide to overall concepts before researching a solution that has to interact with other parts of your Home Theater system.  

You can check our [general software section](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) for what's appropriate depending on what you want to do.

A simple setup may just have a standalone PC with the appropriate software or a [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc). Usually if streaming or a remote-based interface is a priority, then a media device is best, where a PC is better for more customization, local content, keyboard/mouse interaction or lots of storage.  

If a PC, it's normal to want to make the interface as easy to use as a media device and less like a Windows or Linux OS desktop. It will not be all the way there, but you can get partially there either with specialized operating systems, like [LibreElec](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up), a Kodi interface-based OS built mostly for media and emulation, [Bazzite](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up), a SteamOS-like OS built for mostly gaming, other linux-based distros for emulation (like Batocera or Lakka), or just [Launchers](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) over top of Windows/Linux to open Apps; this can be combined with either a [keyboard, remote, or game controller](/wiki/components#keyboardsremotesgamepads).  

Setups vary and there are many ways to do things. Finding the best way for you takes some time and research.  

In the next section are listed some quick-fire pre-built solution recommendations for client and server hardware based on common use-cases. If you're not satisfied with those for your use-case, detailed, complete solutions can be found in the [Building/Buying](/wiki/sample-builds) page, with DiY [components](/wiki/components) in their own page.  

Once you build/buy your solution, you can then follow the recommendations in the [software](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) section and connect/configure things via the [audio](/wiki/audio) and [video](/wiki/video) pages.  

<!-- Section -->

## I want a HTPC/media device recommendation, but don't want to get into the complicated details

Here are recommendations for the most common scenarios, if you don't want to read our whole wiki and/or build something..

Streaming services only: Fire TV 4K stick (Amazon ecosystem) ($40), [Onn 4k Plus](https://www.walmart.com/ip/4K-PLUS-STREAMING/13577404044) (Google ecosystem) ($30)  

Streaming services + 4K local content, no HD audio: Fire TV 4K Max stick ($55), [Onn 4k Pro](https://www.walmart.com/ip/4K-Pro-Streaming-Device/5193222892) (Google ecosystem) ($50). If poor wifi env, add [micro-USB](https://www.amazon.com/Cable-Matters-Streaming-Including-Chromecast/dp/B07N2ZHFY9) or [usb-a](https://www.amazon.com/gp/product/B00BBD7NFU/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) ethernet adapter.  

4K HDR10/Dolby Vision local content + streaming services, HD audio: Nvidia Shield Pro ($200).  

4K HDR local content, HD audio: HDR10: Odroid [N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ($65/$80) / [N150](https://www.amazon.com/s?k=beelink+n150&crid=3CMH2TA4O87KZ&sprefix=beelink+n15%2Caps%2C148&ref=nb_sb_noss_2) ($170) Mini PC. HDR10+/Dolby Vision: Ugoos AM6B Plus (4K)/AM8 Pro (8K) ($200/$250). Both running CoreELEC  

4K HDR10 local content + streaming services + Web Browsing (standard), Windows: Used: Intel i5 8th Gen [NUC (NUC8I5)](https://www.ebay.com/sch/i.html?_nkw=nuc+%288i5%2C8i7%29+-8260u+-8265u&_sacat=179&_from=R40&LH_TitleDesc=1&_sop=15&LH_PrefLoc=2&_blrs=recall_filtering) ($125) OR New: [Asus NUC 14 Essential](https://www.google.com/search?q=nuc+14+essential&oq=nuc+14+essential) ($225) Mini PC 

Cheap Emulation Gaming: Odroid [N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ($80) + EmuElec/Batocera OR Used: >= 
[SFF/USFF PC - CPU >= i5-8500T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini%29+ssd&_sacat=179&_from=R40&_fsrp=1&LH_BIN=1&_sop=15&_udhi=175&_blrs=recall_filtering) ($75)

1080p Casual Gaming: [Beelink SER5 Max (6800U) mini pc](https://www.amazon.com/Beelink-Pro%EF%BC%8CAMD-powerful-Computer-Fingerprint/dp/B0CBTBJWHG?th=1) ($300)

<!-- [Orange Pi 3 LTS 2GB](https://www.aliexpress.us/item/3256804341645667.html) -->

1080p local content, HD audio: **[Odroid C4](https://www.hardkernel.com/shop/odroid-c4/)** / [RPI 4 2GB](https://www.google.com/search?q=raspberry+pi+4+2gb&oq=raspberry+pi+4+2gb) ($50)  

1080p local content + Web Browsing (minimal), Linux: **[Odroid C4](https://www.hardkernel.com/shop/odroid-c4/)** / [ROCK64-4GB](https://pine64.com/product/rock64-4gb-single-board-computer/) ($50)  

1080p local/streaming content + Web Browsing (standard), Windows: Used: >= [SFF/USFF PC - CPU >= i5-8x00T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini%29+ssd&_sacat=179&_from=R40&_fsrp=1&LH_BIN=1&_sop=15&_udhi=175&_blrs=recall_filtering) ($75) OR New: >= [N100 Mini PC](https://www.amazon.com/dp/B0CX14YPTN/ref=twister_B0DC6D6QP7?_encoding=UTF8&th=1) ($150)   

Media Server (no/1080p transcoding): Used: [SFF/USFF PC - CPU >= i5-8x00T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini%29+ssd&_sacat=179&_from=R40&_fsrp=1&LH_BIN=1&_sop=15&_udhi=175&_blrs=recall_filtering) ($75) OR New: >= [N100 Mini PC](https://www.amazon.com/dp/B0CX14YPTN/ref=twister_B0DC6D6QP7?_encoding=UTF8&th=1) ($150)  

Media Server (4k transcoding):  Used: [SFF/USFF PC - CPU >= i5-8x00T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini%29+ssd&_sacat=179&_from=R40&_fsrp=1&LH_BIN=1&_sop=15&_udhi=175&_blrs=recall_filtering) ($75) OR New: >= [N150 Mini PC](https://www.amazon.com/s?k=beelink+n150&crid=3CMH2TA4O87KZ&sprefix=beelink+n15%2Caps%2C148&ref=nb_sb_noss_2) ($170)   

Network Storage: [Storage Setup Guide](/wiki/storage)

Everything else: [Sample Builds/Pre-builts](/wiki/sample-builds)  

*HD Audio means Dolby TrueHD, DTS-HD, DTS:X, and/or Lossless version of Dolby Atmos*

<!-- Section -->

## Asking for help

If you can't find an answer to your question in this FAQ, and are planning to post on the subreddit for help, please give as much information as possible.  

We ask that you answer the following questions and paste them in your post, otherwise your post may be removed for lack of details.  

Do NOT ask for help with playing media on [laptop screens or PC monitors](/wiki/components#displays).

**General Help**

 1. What is the nature of your question/problem? Please be as detailed (but concise) as possible.  

 2. What and how many devices are in your environment (client (pc, media device), server, avr, tv, soundbar)? **Provide model numbers for all the relevant devices**.  

 3. How are the devices connected from an audio/visual perspective? HDMI, optical, etc..  

 4. If applicable, what kind of network are you using? (wifi, wired ethernet, etc..)  

 5. If applicable, what video file codec/resolution/bitrate are you playing/serving (use [mediainfo](https://mediaarea.net/en/MediaInfo))?  

 6. If applicable, what audio file codec are you playing/serving (use [mediainfo](https://mediaarea.net/en/MediaInfo))? PCM, DD, DTS, TrueHD, AAC, Atmos, etc..  

 7. If related to a custom built device, please list all parts of your build.  

 8. What Operating System, software, software versions and software settings are being used?  

 9. Any other relevant information?  

**Build Help**

 1. For what purposes are you using the device (playing/serving media, PC apps, browsing, downloading, gaming)?

 2. Will this device be a client, server, both or standalone?

 3. What types of and how many other client devices will you be using, if any (roku, firetv, shield TV, google cast, tv app, etc..)?

 4. What types of and how many other output, input or misc devices will you be using, if any (tv, avr, soundbar, etc..)?

 5. What types of media will you play/serve? (local, streaming, etc..)? If streaming, what services?

 6. How much media do/will you have (in GB)? Is it/will it be external (NAS) or connected to this device (internal/USB)?

 7. What file types/resolution/bitrate will you be playing/serving?

 8. What type of audio do you need to support? Stereo, DD/DD+, DTS, HD Audio (TrueHD, DTS-HD, Atmos)

 9. What is your budget?

 10. Do you want to build the device or do you want to buy a pre-built solution?

 11. What is your timeframe for implementing the solution?

 12. Any other specific requirements you have (size, noise, power, etc..)?

<!-- Section -->

## What hardware components should I choose for my HTPC?

[See our separate wiki page here](/wiki/components)

<!-- Section -->

## How do i wake/power on/power off my HTPC with a remote/mobile app?

You may want to wake your HTPC from sleep (S3) or have the ability to power it on (S5) or off from your remote control or a mobile app. There are a few ways to do this. Each has its own pros and cons. Keep in mind, turning PCs off and on lowers the life of the components due to thermal and electrical stress.  

1. Wake/Power On/Off: Use HDMI CEC with another HT device. Wake: [Pulse-Eight USB CEC adapter](https://www.pulse-eight.com/p/104/usb-hdmi-cec-adapter), Wake/Power On/Off: [Intel NUC 7+](https://www.intel.com/content/www/us/en/support/articles/000023500/intel-nuc/intel-nuc-kits.html); add HTPC Control: NUC 7/8/10 + [Pulse-Eight Int. CEC](https://www.pulse-eight.com/p/154/intel-nuc-hdmi-cec-adapter).

2. Wake: Use a [Flirc USB](https://flirc.tv/more/flirc-usb) device plugged into your HTPC and an IR remote

3. Wake/Power On/Off: DiY: Use a [Flirc Streacom USB](https://flirc.tv/products/flirc-streacom?variant=43085036486888) device wired into your HTPC mobo and an IR remote. Requires a case with an IR window or drill-modded to allow the IR signal into the module.

4. Wake: Use a HTPC with an IR sensor ([Intel NUC 7/8/11, Asus PN, Gigabyte Brix](/wiki/nuc)) and a [Pepper Jobs W10](https://www.pepper-jobs.com/products/w10-gyro-smart-remote) IR remote

5. Wake/Power On/Off: DiY: Use a Silverstone [ES02](https://www.silverstonetek.com/en/product/expansion-cards/?page=1&filter=Power_OnOff_addon_cards&sort=Newsest) and included remote or [ES03-WIFI](https://www.silverstonetek.com/en/product/expansion-cards/?page=1&filter=Power_OnOff_addon_cards&sort=Newsest) and mobile app

6. Power On/Off: DiY: Use a [Simerec IR Remote Switch](https://www.simerec.com/index.html) and an IR remote  

7. Power On/Off: Plug your HTPC into a [smart power plug](https://www.amazon.com/Assistant-Controlled-Google-Enabled-Vacation/dp/B07XZT24B8). Use with mobile app and/or google/alexa voice tech. If you're IoT-averse, use a [dumb power plug](https://www.amazon.com/DEWENWILS-Control-Wireless-Interference-Programmable/dp/B09X2W2TRT) w/remote instead.

8. Power On/Off: Plug your HTPC into a [power strip with a master/control](https://www.google.com/search?q=sunbeam+advance+7&oq=sunbeam+advance+7) plus and configure your BIOS to set Power On for AC after power loss. Plug master/initial power-on device (like TV) into control port.

9. Wake/Power On: [Configure Wake-on-Lan](https://www.gearrice.com/update/turn-on-a-pc-remotely-with-wake-on-lan-or-remote-control/) in your BIOS and on your network card. Use with a mobile app like Unified Remote

10. Wake: Using a Keyboard/Mouse/Gamepad with a USB dongle/support, Enable Wake/Resume-on-USB and Disable ErP (if available) in your BIOS. In Windows, Disable Fast Startup and Enable Allow Device to Wake Computer under the USB device properties in Device Manager.

11. Wake/Power On/Off: Install a [SwitchBot bot](https://www.switch-bot.com/) on your HTPC's power button. Use SwitchBot Remote or mobile app.

If you want to control other devices from your HTPC, there are a number of ways depending on the target device's capabilities. Potential solutions include taking actions on triggers from Task Scheduler and [EventGhost](https://github.com/EventGhost/EventGhost/releases), combined with actions to devices using hardware like [Pulse-Eight](https://www.pulse-eight.com/p/104/usb-hdmi-cec-adapter) (CEC), [USB-UIRT](http://www.usbuirt.com/) (IR), [Flirc USB](https://flirc.tv/collections/receivers) (IR), [IR Blasters](https://www.iguanaworks.net/products/usb-ir-transceiver/) (IR) and software like [WinLirc](https://winlirc.sourceforge.net/), [EventGhost CEC plugin](https://github.com/sam-6174/pulse-eight-egplugin), [Home Assistant](https://www.home-assistant.io/), [Wake-On-Lan](https://www.nirsoft.net/utils/wake_on_lan.html), and [IFTTT](https://ifttt.com/).  


## Why would I use a PC over a media device (roku, firetv, shield, etc..) for a HTPC?

While media devices are great frontends that are easy to use and navigate, they're not for every scenario. They are best when your usage profile is limited, esp. in terms of the software and hardware you want to use. These are a lot of the reasons you may want to use a PC for your HTPC instead of a media device.  

1. You want to run apps/services on windows or linux, or use a specific, customizable interface, that is/are not available on media device operating systems.  

2. You want to do moderate to extensive web browsing. Media devices, while they can do it, are not good at this from both a HTML spec perspective and for ease of navigation.  

3. You want it to function as a server. You want to provide services like sonarr, radarr, tautulli, plex, VMs, bittorrent.  

4. You want to have more control over video processing; with video renderers like madVR and SVP you can have more control and get better results when doing things like HDR->SDR tonemapping and image, chroma and frame-rate upscaling. You want video refresh rates beyond 60 Hz (e.g. 120 Hz). You need to use multiple displays.  

5. You want more control over audio processing (decoding, mixing, equalization, etc..). You want HD audio (TrueHD/DTS-HD MA, Atmos/DTS:X) that most streaming devices like Roku, FireTV (some), Google TV, (not counting Nvidia Shields or SBCs) don't provide. They'll only do lower quality versions of DD/DTS/Atmos. See [media devices](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) section below for details per device.  

6. You'd rather use a keyboard/mouse instead of a remote for navigation. Media devices are better suited for remote-based navigation. PCs are better suited for keyboard/mouse.  

7. You want to combine HTPC and other computing duties into one machine and/or you don't want to maintain more than one device.  

8. You need more processing power than a streaming device can provide (Local gaming, emulation gaming >= GameCube, VR, etc..)  

9. You like to build things. You'd rather use commodity/DIY hardware/software.  

10. You need more I/O ports or more of a variety of ports (USB, optical, gigabit LAN, 3.5" audio etc..) than most media devices provide and would rather not buy external hardware to do this. You plan to use hardware not supported on a streaming device (USB DAC, TV tuner card. sound card, etc..)  

11. You want to have internal storage rather than external storage.  

12. You have privacy concerns with proprietary systems.  


## What software will I need and how do I set it up?

For the software side of things, there are various tools you may need to take advantage of your HTPC. An OS, media player, media server, ripper, downloader, file renamer, etc.. 

**Operating Systems:** 

Windows, Linux and Android are the most popular choices, as you can imagine. 

If you want to get the highest resolution from [streaming services](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) (esp. DRMed ones), use HDR, video upscaling like madVR, or are combining with a gaming solution, you would use Windows.  

Linux, alternatively, is free and good for local and emulation content, but you will be limited to [lower resolution streaming services](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) and no stable HDR. Ubuntu and Fedora are good distros to start with.

There are some specialized linux-based distros out there, like [LibreElec (x86)](https://libreelec.tv/)/[CoreElec (ARM)](https://coreelec.org) which are OSes designed for running Kodi as the OS's plugin-capable front interface. They're very good for local content, emulation and game streaming, even HDR and work well with a [simple remote/controller](/wiki/components#keyboardsremotesgamepads). Like stock linux, they also suffer from lower resolutions on streaming services.  

For Android ports to PC look at [Android x86](https://www.android-x86.org/) or [Bliss OS](https://blissos.org/), but do not expect a TV-like interface, 4K streaming services or HD audio. You can run an Android container under Linux with [Waydroid](https://waydro.id/) and under Windows with [WSABuilds](https://github.com/MustardChef/WSABuilds). 

For a gaming-centric OS, look at the SteamOS-like [Bazzite](https://docs.bazzite.gg/General/Installation_Guide/Installing_Bazzite_for_HTPC_Setups/) or [ChimeraOS](https://chimeraos.org/). You can combine this with [EmuDeck](https://www.emudeck.com) for emulation or Plex/Kodi/VLC for media.  

**Launchers:** 

For a launcher interface to open multiple apps, look at:
 - [Flex Launcher](https://complexlogic.github.io/flex-launcher) (Windows/Linux)
 - [TV Launcher](https://github.com/Darkvinx88/TvLauncher) (Windows/Linux)
 - [Steam Big Picture mode](https://store.steampowered.com/bigpicture) (Windows/Linux/Mac)
 - [Kodi](https://kodi.wiki/view/Archive:HOW-TO:Make_Windows_boot_directly_to_Kodi_(as_a_shell)) with [add-ons](https://kodi.wiki/view/Category:All_add-ons) for pvr, emulators, etc..
 - [Omnimo for Rainmeter](https://omnimo.info/) (Windows)
 - [Plasma Bigscreen](https://plasma-bigscreen.org/) (Linux)
 - [Windows 10 start menu in full screen mode](https://www.reddit.com/r/htpc/comments/92ek4d/homescreen_for_htpc_and_ideas_for_what_i_can_put/e356duu/)
 - [Windows tablet mode](https://www.tenforums.com/tutorials/3755-turn-off-tablet-mode-windows-10-a.html)

**Media Players:** 

For [video streaming services](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x), use Microsoft Edge to get 1080p+, or the service's app (if available).  

For simple media players, using local content, [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases), [VLC](https://www.videolan.org/vlc/) and [MPC-HC](https://github.com/clsid2/mpc-hc/releases/) are popular on Windows, with [Kodi](http://kodi.tv/) and [VLC](https://www.videolan.org/vlc/) on Linux.  

If [simple HDR passthrough/tomemapping](/wiki/hdr) is what you're looking for, then look at [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases) with the built-in MPCVR renderer or [Kodi](http://kodi.tv/).  
For [high-end video upscaling or HDR tonemapping](/wiki/hdr), look at MPC-BE/MPC-HC with the madVR renderer.  
For FPS upscaling, the [SmoothVideo Project](https://www.svp-team.com/).  

But perhaps you want a more full-featured player/interface..  

If you DON'T need to serve media to other devices and just want a well-supported, highly-customizable home theater front-end, look at [Mediaportal](http://www.team-mediaportal.com/), [Jriver Media Center](https://www.jriver.com/) or [Kodi](http://kodi.tv/). All three will pull down metadata for the media you point them to, keep track of what you have watched/haven't watched, keep playback progress, pass-through HDR, and play from your internal or network storage. For Kodi, start with Kodi's [First Time User guide](https://kodi.wiki/view/First_time_user) and 3rd party guides like [this](https://androidpcreview.com/how-to-setup-kodi-the-right-way/).  
If you DO need to serve media to other devices (local or remote) and/or want centralized metadata management, see Plex/Jellyfin/Emby client/server solutions in Media Servers below.

For playback of 3D MVC/Frame-Packed/SBS content, [See our separate wiki page here](/wiki/3d)  

**Gaming/Emulation:** 

For Game Emulation, look at:
  - Linux: [Batocera](https://batocera.org/), [LibreElec](https://libreelec.tv/downloads/) w/Retroarch, or [Lakka (RetroArch on a stick)](https://www.lakka.tv/) 
  - Windows: [RetroArch](https://www.retroarch.com/?page=platforms), [EmulationStation DE](https://es-de.org/) or [Launchbox Big Box](https://www.launchbox-app.com/premium) 
  - Bazzite: [Emudeck](https://www.emudeck.com) 
  - Mac: RetroArch or [OpenEmu](https://openemu.org/) 
  - Android: [Lemuroid](https://play.google.com/store/apps/details?id=com.swordfish.lemuroid&hl=en_US&gl=US) or RetroArch 
  - Apple TV: [Provenance](https://github.com/Provenance-Emu/Provenance) 
  - Others: [Nostlan](https://github.com/quinton-ashley/nostlan) for large 4k displays.

For Game Streaming, look at [Sunshine](https://app.lizardbyte.dev/Sunshine) on your server/gaming PC and [Moonlight](https://moonlight-stream.org/) on your frontend client ([Windows/Linux/Android](https://github.com/moonlight-stream/moonlight-qt)/[LibreElec](https://github.com/veldenb/plugin.program.moonlight-qt)/tvOS).  

For Gaming, look at Steam w/Windows or Linux, as well as [Bazzite](https://universal-blue.discourse.group/t/bazzite-inital-setup-and-installation-for-htpc-setups/1145) or [ChimeraOS](https://chimeraos.org/) for a whole Steam-based OS.  

**Media Servers:** 

[Plex Media Server](https://www.plex.tv) is very popular and will index your media, pull metadata (like cover art/plot/cast/tv show data), track what you have watched/haven't watched and stream it out to your client devices. It also has a [wide range of player apps](https://www.plex.tv/media-server-downloads/#plex-app) to install on your client devices. For PC specifically, there is Plex HTPC (keybrd/remote-based) and Plex for Windows (mouse-based). If you don't like the plex-branded ones, you can, alternatively, integrate the [Kodi](https://kodi.tv/addons/matrix/script.plex) player with the Plex server. For alternatives to Plex Media Server, there is [Emby](http://emby.media/) and [Jellyfin](https://jellyfin.org/). See our [dedicated section](/wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device) for more information. 

**Organization:** 

To organize your content, look at Radarr (movies), Sonarr (tv), Lidarr (music) and Bazarr (subtitles). You can use these together to keep your content in properly named files/folders for Plex, retrieve subtitles and show you what content you have or don't have. You can interface with these using their respective web interfaces or with an app like [nzb360](https://play.google.com/store/apps/details?id=com.kevinforeman.nzb360&hl=en_US&gl=US) on an android device. For metadata management, look at [Media Hoarder](https://media.hoarder.software). For file management, look at [Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) [w/LAN plugin](https://play.google.com/store/apps/details?id=com.ghisler.tcplugins.LAN) or [X-Plore](https://www.lonelycatgames.com/apps/xplore).  

For an overall sense of how a basic HTPC platform should look with playback, serving, storage, and organization, look at our [diagram here](https://i.imgur.com/gUI1R6z.png).  

For a comprehensive guide to setting up all the backend organizational/serving software, the [HTPC Box Guide](https://github.com/sebgl/htpc-download-box) will take you through a modern installation approach to the stack using Linux & Docker containers. The [TRaSH Guide](https://trash-guides.info/Hardlinks/How-to-setup-for/) is a good supplement to this. For Windows, we can recommend [The Ultimate Server Guide](http://www.cuttingcords.com/home/ultimate-server/getting-started); even though it's old, the concepts are the same. The [Servarr Wiki](https://wiki.servarr.com/) is a great reference for all the \*arr software.  

**Other software:** 

For Live TV software, see the [dedicated section](/wiki/faq#can-i-watch-live-tv-or-record-it-and-play-it-back-on-my-htpc) below.  

For Optical disc playback, see the [dedicated section](/wiki/faq#how-can-i-play-my-dvdblu-ray-discs-on-my-htpc) below.  

For Optical disc ripping and transcoding, see the [dedicated section](/wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use) below.  

If you're planning on replacing cable/sat with similar streaming services, you will find [r/cordcutters](https://www.reddit.com/r/cordcutters/) to be helpful.  

If you'd like to have a podcast, audio podcast or audiobook library in Plex, [see this handy guide](http://www.reddit.com/r/PleX/comments/3avpi9/how_to_create_a_podcast_library_a_video_podcast/).  

[This page](http://kodi.wiki/view/Supplemental_tools) has a list of additional, supplemental software relating to HTPCs.

## Can I use my HTPC for streaming from services such as Netflix, Youtube, Amazon, Hulu, etc..? 

Yes, however the interface quality and functionality varies widely and remote control support is almost non-existent. The services will detect your device as a PC and present you with their standard web or app-based interface. It may be up to you to start videos and expand them to full-screen.  

Video/audio support for streaming services in general is limited on a traditional HTPC. See our sections on [streaming service support and setup](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) and [4K compatibility](/wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility).  

Using Windows Store apps for some of these services may be better than using a web browser in terms of video/audio support. 

For example, the Netflix Windows Store app does support 4k/1080p streaming and Dolby Digital/Dolby Digital Plus soundtracks. Browser-based solutions other than Microsoft Edge tend not support DD/DD+ audio and some content will only be available in 720p. The app still does not have remote control support, but you can try adding 3rd party remote control support using the [Netflix Remote Controller](http://sticky-ux.com/apps/NetflixRemoteController/).  

Support for the higher resolutions and audio is way more prevalent on pre-built media devices, so if you use a lot of these services, it's better NOT to use a PC. See our [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) section below for options.  

In regards to internet bandwidth required, you should have 6 Mbps downstream to stream 1080p services. 25 Mbps for 4k.  

If you don't plan on using a [keyboard/mouse-like device](/wiki/components#keyboardsremotesgamepads), then streaming services on a PC will be painful. There are some good workarounds like [software](/wiki/components#keyboardsremotesgamepads) to emulate a mouse on game controllers/mobile, like Controller Companion with an 8bitdo Ultimate 2c controller.  

Other possible solutions are:  
* Youtube: [VacuumTube](https://github.com/shy1132/VacuumTube) OR <code>"%PROGRAMFILES%\Google\Chrome\Application\chrome.exe" --kiosk --enable-extensions --user-agent=Xbox https://www.youtube.com/tv</code> OR [Leanback interface](https://redd.it/y5o7mi)
* Netflix: <code>"%PROGRAMFILES%\Google\Chrome\Application\chrome.exe" --kiosk --enable-extensions https://www.netflix.com</code> + [Netflix Navigator](https://netflixnavigator.com) extension
* Other services: Browser Kiosk mode (<code>"%PROGRAMFILES(X86)%\Microsoft\Edge\Application\msedge.exe" --kiosk --edge-kiosk-type=fullscreen</code>) + [TamperMonkey](https://www.tampermonkey.net/) extension + [Stream Assistant](https://github.com/CHJ85/Stream-Assistant) script
* Keyboard Macros: [AutoHotKey](https://www.autohotkey.com)
* Launcher: [Flex Launcher](https://github.com/complexlogic/flex-launcher)

If those things aren't good enough for you, then you should buy a remote-based [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) from the next section instead.  

## Can I use a pre-built media device for my HTPC?

Yes, you can. There are many already-built devices out there. Media devices from major brands like Roku/Amazon/Google/Apple/Nvidia/Roku will have better support for video resolutions/HDR than a traditional HTPC. See the next section/question for why you would choose one device or brand over another. <!-- There is also a list of popular devices at [wikipedia](https://en.wikipedia.org/wiki/Comparison_of_digital_media_players) which gives further information like supported streaming apps. -->  

Beware of cheap no-name android boxes on obscure websites. They likely will have no or poor support and very little documentation if you run into trouble.  

If you're looking for the best Plex client, watch [this](https://www.youtube.com/watch?v=qLxjL2NxZy8) video for tests on loading/scrolling/playing/audio/remotes/etc..  

If you want a traditional standalone HTPC see the Mini PCs at the end of the list or our [Sample Builds](/wiki/sample-builds) page for more extensive options.  

Legend: PT: Passthrough, DC: Decode, LS: Lossy, LL: LossLess, DD: Dolby Digital, DV: Dolby Vision, DA: Dolby Atmos, DTHD: Dolby TrueHD, DV-5: Dolby Vision - Streaming Services, DV-7M/7F: Dolby Vision Disc Rips - 7M (MEL)/7F (FEL), EOL: End of Life, V: Video, A: Audio

<!--
BRAND/MODEL|PRICE|RESOLUTION|4k NETFLIX?|HDR?|WIFI?|LAN?|VOICE SEARCH?|USB?|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
[Raspberry Pi 4b](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/) / [5](https://www.raspberrypi.com/products/raspberry-pi-5/) ([buy](https://www.pishop.us/product/raspberry-pi-4-model-b-1gb/)/[buy](https://www.pishop.us/product/raspberry-pi-5-4gb/))|$36/$60|4k@60 (2,4)|No|10/HLG (2)|ac|1000M|No|YES (8b)|HDR10/HLG, LL DA/DTSX w/LibreElec, BT 5.0
[Odroid C4](https://www.hardkernel.com/shop/odroid-c4/) ([buy](https://www.hardkernel.com/shop/odroid-c4/))|$55|4k@60|No|10 (6)|Opt|1000M|No|YES (8b)|S905X3/4GB RAM. PT:**LL DA/DTSX** w/CoreElec
[Odroid N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ([buy](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/))|$66|4k@60|No|10 (6)|Opt|1000M|No|YES (8b)|S922x/2GB RAM/8 GB SD. PT:**LL DA/DTSX** w/CoreElec
[Dune HD Box R Plus](https://www.dune-hd.com/products/homatics-box-r-4k-plus) ([buy](https://www.dune-hd.com/products/homatics-box-r-4k-plus))|$150|4k@60|No|10/+/DV (6)|ax|1000M|No|YES (8b)|S905X4-K/4GB RAM/32 GB SD. **DV-5/7/8**, PT:**LL DA/DTSX** w/CoreElec
[Mi Box S](https://www.mi.com/global/mi-box-s) ([buy](https://www.amazon.com/Xiaomi-Android-Google-Assistant-Streaming/dp/B07KLWGGYS))|$65|4k@60|YES|10|ac|No|YES|YES (**8b**)|PT:LS DD+/DTS, S905X-H/2GB/8GB, NTFS
**[Apple TV 4k (2022)](https://www.apple.com/apple-tv-4k/)** ([buy](https://www.apple.com/shop/buy-tv/apple-tv-4k))|**$129/$149**|4k@60|YES|10/+/DV|ax|1000M (7)|YES|No|3rd gen, A15, 3GB/64-128GB, DV-5/8, DC:DTHD/DTSHD->PCM, PT:LS DA, BT 5.0
[Onn 4K](https://www.walmart.com/ip/onn-Google-TV-4K-Streaming-Box-New-2023-4K-UHD-resolution/2835618394) ([buy](https://www.walmart.com/ip/onn-Google-TV-4K-Streaming-Box-New-2023-4K-UHD-resolution/2835618394))|$20|4k@60|YES|10|dual ac|Opt (9a)|YES|Opt (8a)|DC:NA, PT:LS DD/DTS, S905Y4 1.9Ghz/2GB/8GB
**[Onn 4K Pro](https://www.walmart.com/ip/4K-Pro-Streaming-Device/5193222892)** ([buy](https://www.walmart.com/ip/4K-Pro-Streaming-Device/5193222892))|**$50**|4k@60|YES|10/+/DV|ax|100M, Opt (9c)|YES|Opt (8c)|DC:NA, PT:LS DA/DTS, S905X4 2Ghz/3GB/32GB
[ChromeCast w/Google TV 4k](https://store.google.com/product/chromecast_google_tv) ([buy](https://store.google.com/config/chromecast_google_tv))|$50|4k@60|YES|10/+/DV|dual ac|Opt (9b)|YES|Opt (8a)|2nd gen. AV1, DV-5/8, DC:DD+, PT:LS DA/DTS, S905D3 1.9Ghz/2GB/8GB
[Google TV Streamer 4k](https://store.google.com/us/product/google_tv_streamer?hl=en-US) ([buy](https://store.google.com/us/product/google_tv_streamer?hl=en-US))|$100|4k@60|YES|10/+/DV|dual ac|1000M|YES|Opt (8c)|3rd/latest gen. AV1, DV-5/8, DC:LS DA/DTHD/DTSHD->PCM, PT:LS DA/DTS, MT8696/4GB/32GB
**[Amazon Fire TV stick 4K MAX (2023)](https://www.amazon.com/dp/B0BP9SNVH9)** ([buy](https://www.amazon.com/dp/B0BP9SNVH9))|**$60**|4K@60|YES|10/+/DV|tri ax 2x2-6e|Opt (9a)|YES|Opt (8a)|2nd gen, AV1, DV-4/5/8/9/10, PT:**LL DA**/DTSHD, 2.0Ghz/2GB/16GB
[Amazon Fire TV stick 4K MAX (2021)](https://www.amazon.com/dp/B08MQZXN1X) ([buy](https://www.amazon.com/dp/B08MQZXN1X))|$55|4K@60|YES|10/+/DV|dual ax 2x2-6|Opt (9a)|YES|Opt (8a)|1st gen, AV1, PT:LS DA, 1.8Ghz/2GB/8GB
[Amazon Fire TV stick 4K (2023)](https://www.amazon.com/dp/B0CDR2MSVC) ([buy](https://www.amazon.com/dp/B0CDR2MSVC))|$40|4K@60|YES|10/+/DV|dual ax 2x2-6|Opt (9a)|YES|Opt (8a)|2nd gen, DV-4/5/8/9/10, PT:**LL DA**, 1.7Ghz/2GB/8GB
[Amazon Fire TV stick](https://www.amazon.com/dp/B07ZZVX1F2/B08C1W5N87) ([buy](https://www.amazon.com/dp/B07ZZVX1F2/B08C1W5N87))|$40|1080p|NO|10/+|dual ac 2x2|Opt (9a)|YES|Opt (8a)|3rd Gen, DC: LS DA, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[Amazon Fire TV stick Lite](https://www.amazon.com/dp/B091G4YP57) ([buy](https://www.amazon.com/dp/B091G4YP57))|$30|1080p|NO|10/+|dual ac 2x2|Opt (9a)|YES|Opt (8a)|BT 5.0 LE, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[Amazon Fire TV cube](https://www.amazon.com/dp/B0BFD4M9C8) ([buy](https://www.amazon.com/dp/B0BFD4M9C8))|$140|4K@60|YES|10/+/DV|tri ax 2x2-6E|10/100 (9a)|YES|YES (**8b**)|3rd gen, AV1, PT:**LL DA**/DTSHD,DC:LL DA->PCM, 2.2Ghz/2GB/16GB, NTFS
[Roku Express](https://www.roku.com/products/roku-express) ([buy](https://smile.amazon.com/Roku-Express-Streaming-Media-Player/dp/B07WVFCVJN))|$25|1080p|NO|NO|n|No|No|No|DD, PT:LS DTS/DA
[Roku Express 4K](https://www.roku.com/products/roku-express-4k)/[+](https://www.roku.com/products/roku-express-4k-plus) ([buy](https://www.walmart.com/ip/Roku-Express-4K-2021-Streaming-Media-Player-HD-4K-HDR-with-Smooth-Wireless-Streaming-and-Simple-Remote-includes-Premium-HDMI-Cable/651641821)/[buy](https://amzn.to/3g56Djl))|$35/$40|4k@60|YES|10/+|dual ac|No/Opt|No/YES|Opt|DC:DD/PT:LS DTS/DA
**[Roku Streaming 4K](https://www.roku.com/products/roku-streaming-stick-4k)** ([buy](https://www.amazon.com/Roku-Streaming-Device-Vision-Controls/dp/B09BKCDXZC))|**$50**|4k@60|YES|10/+/DV|dual ac 2x2|No|YES|No|1GB, DC:DD/PT:LS DTS/DA. Model: 3820R2
[Roku Ultra](https://www.roku.com/products/roku-ultra) ([buy](https://www.amazon.com/Roku-Ultra-2024-Streaming-Rechargeable/dp/B0DF44RTTP))|$100|4k@60|YES|10/+/DV|ax|100M|YES|YES (**8b**)|2GB RAM, DC:DA, PT:LS DTS/DA, AV1, NTFS. Model: 4850R
[Roku Ultra LT](https://www.roku.com/products/roku-ultra-lt) ([buy](https://www.walmart.com/ip/Roku-Ultra-LT-Streaming-Media-Player-2019/857445471))|$80|4k@60|YES|10|dual ac|100M|YES|No|2GB RAM, DC:DD+, PT:LS DTS/DA. Model: 4801RW
[Vero V](https://osmc.tv/vero/) ([buy](http://buy.getvero.tv/))|$150|4k@60|No|10/+|ac|1000M|No|YES (**8b**)|OSMC, PT:**LL DA**/DTSX, 2Ghz/4GB/32GB, NTFS
[Nvidia Shield TV Tube](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP94PBJ))|$150|4k@60|YES|10/DV|ac|1000M|YES|No|DV-5/7/8, PT:LL DA/DTSX DC:DA, 2GB/8GB, NTFS, microSD
**[Nvidia Shield TV Pro](https://www.nvidia.com/en-us/shield/shield-tv-pro/)** ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP9FBMM))|**$199**|4k@60|YES|10/DV|ac|1000M|YES|YES (**8b**)|**DV-5/7/8**, PT:**LL DA/DTSX** DC:DA, 3GB/16GB, NTFS
[Nvidia Shield TV (2017)](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-SHIELD-Gaming-Streaming-GeForce/dp/B075RXV2VR))|$179|4k@60|YES|10|ac|1000M|YES|YES (8b)|PT:**LL DA/DTSX**, 16GB, NTFS
[Xbox One S/X](https://www.xbox.com/en-US/xbox-one/consoles) ([buy](https://smile.amazon.com/gp/bestsellers/electronics/6469295011))|$200-$400|4k@60|YES|10/DV|dual-ac|1000M|No|YES (8b)|PT:LL DA/DTSX, 1TB, UHD-BR
Mini PC: i3/i5-8x00T ([buy](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28dell%29+%28i3-8100%2Ci5-8400%2Ci5-8500%29&_sacat=179&LH_TitleDesc=0&LH_BIN=1&_sop=15&_udhi=150&_blrs=recall_filtering))|$100|4k@60 (10a)|YES|10|n/ac|1000M|NO|YES (8b)|PT:**LL DA/DTSX**
Mini PC: Intel N100 ([buy](https://www.amazon.com/s?k=n95+n100+mini+pc&crid=GPL0MOIHFBH&sprefix=n95+n100+mini+p%2Caps%2C102&ref=nb_sb_noss_2))|$150|4k@60|YES|10|ac|1000M|NO|YES (8b)|AV1, PT:**LL DA/DTSX**. w/RAM&SSD
Mini PC: [Intel NUC i3/i5/i7](https://www.intel.com/content/www/us/en/products/boards-kits/nuc.html) ([buy](https://www.newegg.com/p/pl?N=100008345%20601398037%20601398023%20601398021%20601398031%20601407140%20601398048%20601398010%20601398014%20601398049%20601398018%20601398044%20601398008%20601398042%20601398025%20601398029%20601398043%20601398019%2050001157&SrchInDesc=-hunsn%2C-Aittact&Order=1))|$300-$900|4k@60|YES|10|ac|1000M|NO|YES (8b)|AV1 (3), PT:**LL DA**/DTSX. add $45 for 8GB RAM/128GB SSD
-->

<!-- START:TEST -->

BRAND/MODEL|PRICE|RESOLUTION|4k NETFLIX|HDR|WLAN/LAN|VOICE|USB|RATING|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
[Raspberry Pi 4b](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/) / [5](https://www.raspberrypi.com/products/raspberry-pi-5/) ([buy](https://www.pishop.us/product/raspberry-pi-4-model-b-1gb/)/[buy](https://www.pishop.us/product/raspberry-pi-5-4gb/))|$36/$60|4k@60 (2,4)|No|10/HLG (2)|ac/1000M|No|YES (8b)|V:Good A:**Best**|HDR10/HLG, LL DA/DTSX w/LibreElec, BT 5.0
[Odroid C4](https://www.hardkernel.com/shop/odroid-c4/) ([buy](https://www.hardkernel.com/shop/odroid-c4/))|$55|4k@60|No|10/+ (6a)|Opt/1000M|No|YES (8b)|V:Good A: **Best**|S905X3/4GB RAM. PT:**LL DA/DTSX** w/CoreElec
[Odroid N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ([buy](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/))|$66|4k@60|No|10/+ (6a)|Opt/1000M|No|YES (8b)|V:Good A:**Best**|S922x/2GB RAM/8 GB SD. PT:**LL DA/DTSX** w/CoreElec
[Dune HD Box R Plus](https://www.dune-hd.com/products/homatics-box-r-4k-plus) ([buy](https://www.dune-hd.com/products/homatics-box-r-4k-plus))|$150|4k@60|YES|10/+/DV (6b)|ax/1000M|No|YES (8b)|V:**Best** A:**Best**|AV1, S905X4-K/4GB RAM/32 GB SD. **DV-5/7F/8**, PT:**LL DA/DTSX**
[Xiaomi TV Box S](https://www.mi.com/global/product/xiaomi-tv-box-s-3rd-gen/) ([buy](https://www.amazon.com/Xiaomi-TV-Box-3rd-Gen/dp/B0F3JWFL56))|$75|4k@60|YES|10/+/DV|ax/Opt (9c)|YES|YES (8c)|V:Better A:**Best**|3rd gen, AV1, DV-5, PT:**LL DA/DTSX**, S905X5M/2GB/32GB, BT 5.2
**[Apple TV 4k (2022)](https://www.apple.com/apple-tv-4k/)** ([buy](https://www.apple.com/shop/buy-tv/apple-tv-4k))|**$129/$149**|4k@60|YES|10/+/DV|ax/1000M (7)|YES|No|V:Better A:Better|3rd gen, A15, 3GB, DV-5/8, DC:DTHD/DTSHD->PCM, PT:LS DA, BT 5.0
[Onn 4K](https://www.walmart.com/ip/onn-Google-TV-4K-Streaming-Box-New-2023-4K-UHD-resolution/2835618394) ([buy](https://www.walmart.com/ip/onn-Google-TV-4K-Streaming-Box-New-2023-4K-UHD-resolution/2835618394))|$20|4k@60|YES|10|ac/Opt (9a)|YES|Opt (8a)|V:Good A:Good|AV1, DC:NA, PT:LS DD/DTS, S905Y4 1.9Ghz/2GB/8GB
[Onn 4K Plus](https://www.walmart.com/ip/4K-PLUS-STREAMING/13577404044) ([buy](https://www.walmart.com/ip/4K-PLUS-STREAMING/13577404044))|$30|4k@60|YES|10/+/DV|ax/Opt (9a)|YES|Opt (8c)|V:Good A:Good|AV1, DC:NA, PT:LS DA/DTS, S905X5M 2.5Ghz/2GB/16GB
**[Onn 4K Pro](https://www.walmart.com/ip/4K-Pro-Streaming-Device/5193222892)** ([buy](https://www.walmart.com/ip/4K-Pro-Streaming-Device/5193222892))|**$50**|4k@60|YES|10/+/DV|ax/100M, Opt (9c)|YES|YES (8c)|V:Better A:Good|AV1, DC:NA, PT:LS DA/DTS, S905X4 2Ghz/3GB/32GB
[ChromeCast w/Google TV 4k](https://store.google.com/product/chromecast_google_tv) (EOL)|$50|4k@60|YES|10/+/DV|ac/Opt (9b)|YES|Opt (8a)|V:Better A:Good|2nd gen. AV1, DV-5/8, DC:DD+, PT:LS DA/DTS, S905D3 1.9Ghz/2GB/8GB
[Google TV Streamer 4k](https://store.google.com/us/product/google_tv_streamer?hl=en-US) ([buy](https://store.google.com/us/product/google_tv_streamer?hl=en-US))|$100|4k@60|YES|10/+/DV|ac/1000M|YES|Opt (8c)|V:Better A:Good|3rd/latest gen. AV1, DV-5/8, DC:LS DA/DTHD/DTSHD->PCM, PT:LS DA/DTS, MT8696/4GB/32GB
**[Amazon Fire TV stick 4K MAX (2023)](https://www.amazon.com/dp/B0BP9SNVH9)** ([buy](https://www.amazon.com/dp/B0BP9SNVH9))|**$60**|4K@60|YES|10/+/DV|ax(E)/Opt (9a)|YES|Opt (8a)|V:Better A:Better|2nd gen, AV1, DV-5/8, PT:**LL DA**/DTSHD, 2.0Ghz/2GB/16GB
[Amazon Fire TV stick 4K Plus (2023)](https://www.amazon.com/dp/B0F7Z4QZTT) ([buy](https://www.amazon.com/dp/B0F7Z4QZTT))|$50|4K@60|YES|10/+/DV|ax/Opt (9a)|YES|Opt (8a)|V:Better A:Better|2nd gen, AV1, DV-5/8, PT:**LL DA**/DTSHD, 1.7Ghz/2GB/8GB
[Amazon Fire TV stick 4K Select (2025)](https://www.amazon.com/dp/B0C6W3D4RM) ([buy](https://www.amazon.com/dp/B0C6W3D4RM))|$40|4K@60|YES|10/+|ac/Opt (9a)|YES|Opt (8a)|V:Good A:Good|1st Gen, AV1, DC: LS DD+, PT:LS DA/DTSHD, 1.7Ghz/1GB/8GB
[Amazon Fire TV stick HD (2024)](https://www.amazon.com/dp/B07ZZVX1F2/B08C1W5N87) ([buy](https://www.amazon.com/dp/B07ZZVX1F2/B08C1W5N87))|$35|1080p|NO|10/+|ac/Opt (9a)|YES|Opt (8a)|V:Good A:Good|DC: LS DD+, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[Amazon Fire TV cube](https://www.amazon.com/dp/B0BFD4M9C8) ([buy](https://www.amazon.com/dp/B0BFD4M9C8))|$140|4K@60|YES|10/+/DV|ax/100 (9a)|YES|YES (**8b**)|V:Better A:Better|3rd gen, AV1, DV-5/8, PT:**LL DA**/DTSHD,DC:LL DA->PCM, 2.2Ghz/2GB/16GB, NTFS
[Roku Express](https://www.roku.com/products/roku-express) ([buy](https://smile.amazon.com/Roku-Express-Streaming-Media-Player/dp/B07WVFCVJN))|$25|1080p|NO|NO|n/No|No|No|V:Good A:Good|DD, PT:LS DTS/DA
[Roku Express 4K](https://www.roku.com/products/roku-express-4k)/[+](https://www.roku.com/products/roku-express-4k-plus) ([buy](https://www.walmart.com/ip/Roku-Express-4K-2021-Streaming-Media-Player-HD-4K-HDR-with-Smooth-Wireless-Streaming-and-Simple-Remote-includes-Premium-HDMI-Cable/651641821)/[buy](https://amzn.to/3g56Djl))|$35/$40|4k@60|YES|10/+|ac/Opt|No/YES|Opt|V:Good A:Good|DC:DD/PT:LS DTS/DA
[Roku Streaming](https://www.roku.com/products/players/roku-streaming-stick)/[Plus](https://www.roku.com/products/players/roku-streaming-stick-plus) ([buy](https://www.amazon.com/Roku-Streaming-Stick-2025-Device/dp/B0DXXYS4BJ)/[buy](https://www.walmart.com/ip/Roku-Streaming-Stick-Plus-2025-4K-HDR-Roku-Streaming-Device-for-TV-with-Voice-Remote-Free-Live-TV/13520604925?classType=REGULAR))|$30/$40|1080p/4k@60|NO/YES|NO,10/+/HLG|n/ac|YES|No|V:Good A:Good|DC:DD/PT:LS DTS/DA. 3830R/3840R. Replace Express
**[Roku Streaming 4K](https://www.roku.com/products/roku-streaming-stick-4k)** ([buy](https://www.amazon.com/Roku-Streaming-Device-Vision-Controls/dp/B09BKCDXZC))|**$50**|4k@60|YES|10/+/DV|ac/No|YES|No|V:Better A:Good|1GB, DC:DD/PT:LS DTS/DA. Model: 3820R2
[Roku Ultra](https://www.roku.com/products/roku-ultra) ([buy](https://www.amazon.com/Roku-Ultra-2024-Streaming-Rechargeable/dp/B0DF44RTTP))|$100|4k@60|YES|10/+/DV|ax/100M|YES|YES (**8b**)|V:Better A:Good|2GB RAM, DC:DA, PT:LS DTS/DA, AV1, NTFS. Model: 4850R
[Roku Ultra LT](https://www.roku.com/products/roku-ultra-lt) ([buy](https://www.walmart.com/ip/Roku-Ultra-LT-Streaming-Media-Player-2019/857445471))|$80|4k@60|YES|10|ac/100M|YES|No|V:Good A:Good|2GB RAM, DC:DD+, PT:LS DTS/DA. Model: 4801RW
[Vero V](https://osmc.tv/vero/) ([buy](http://buy.getvero.tv/))|$150|4k@60|No|10/+|ac/1000M|No|YES (**8b**)|V:Good A:**Best**|OSMC, PT:**LL DA**/DTSX, 2Ghz/4GB/32GB, NTFS
[Nvidia Shield TV Tube](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP94PBJ))|$150|4k@60|YES|10/DV|ac/1000M|YES|No|V:Better A:**Best**|DV-5/7M/8, PT:LL DA/DTSX DC:DA, 2GB/8GB, NTFS, microSD
**[Nvidia Shield TV Pro](https://www.nvidia.com/en-us/shield/shield-tv-pro/)** ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP9FBMM))|**$199**|4k@60|YES|10/DV|ac/1000M|YES|YES (**8b**)|V:Better A:**Best**|**DV-5/7M/8**, PT:**LL DA/DTSX** DC:DA, 3GB/16GB, NTFS
[Nvidia Shield TV (2017)](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-SHIELD-Gaming-Streaming-GeForce/dp/B075RXV2VR))|$179|4k@60|YES|10|ac/1000M|YES|YES (8b)|V:Better A:**Best**|PT:**LL DA/DTSX**, 16GB, NTFS
[Xbox One S/X](https://www.xbox.com/en-US/xbox-one/consoles) ([buy](https://smile.amazon.com/gp/bestsellers/electronics/6469295011))|$200-$400|4k@60|YES|10/DV|ac/1000M|No|YES (8b)|V:Better A:**Best**|PT:LL DA/DTSX, 1TB, UHD-BR
Mini PC: Optiplex ([buy](/wiki/sample-builds#4k-hdr-players))|$100|4k@60 (10a)|YES|10|ax/1000M|NO|YES (8b)|V:Better A:**Best**|HEVC, PT:**LL DA/DTSX**
Mini PC: Beelink EQR6 (6600) ([buy](/wiki/sample-builds#4k-hdr-players))|$270|4k@60|NO|10|ax/1000M|NO|YES (8b)|V:Better A:**Best**|AV1, PT:**LL DA/DTSX**
Mini PC: NUC i3/i5/i7 ([buy](/wiki/sample-builds#4k-hdr-players))|$300-$700|4k@60|YES|10|ax/1000M|NO|YES (8b)|V:Better A:**Best**|AV1 (3), PT:**LL DA/DTSX**, HDMI-CEC

<!-- FINISH:TEST -->

(2) 4k and HDR support using [LibreElec](https://libreelec.tv) >= 10.0.2 and Kodi 

(3) >= 11th gen

(4) Anything other than HEVC is supported at only 1080p

(6a) Running CoreELEC/Libreelec, (6b) Running CoreELEC for DV 7 FEL

(7) 128GB model 

(8a) FAT32, (8b) NTFS+EXFAT+FAT32, (8c) EXFAT+FAT32. "Opt" devices must use [OTG](https://www.amazon.com/s?k=OTG+power+cable&i=electronics) cable 

(9a) micro-usb [Ethernet Adapter](https://www.amazon.com/Cable-Matters-Streaming-Including-Chromecast/dp/B07N2ZHFY9/), (9b) usb-c [Ethernet Adapter](https://www.amazon.com/Cable-Matters-Gigabit-Ethernet-Charging/dp/B08NXS46DN), (9c) usb-a [Ethernet Adapter](https://www.amazon.com/gp/product/B00BBD7NFU/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1). <= 350 Mbps 

(10a) w/[HDMI 2.0 card](https://www.ebay.com/sch/i.html?_from=R40&_nkw=dell+hdmi+2.0+%28HXPK2%2C1KNYY%2CR07CP%2C5N1NY%29&_sacat=0&_sop=12) 

<!--
DISCONTINUED
[ChromeCast w/Google TV HD](https://store.google.com/product/chromecast_google_tv) ([buy](https://store.google.com/product/chromecast_google_tv))|$30|1080p|No|10/+|dual ac|Opt|YES|Opt (8a)|AV1, DC:DD+, PT:LS DA/DTS, S805X2, 1.5GB/8GB
[Apple TV 4k (2021)](https://www.apple.com/apple-tv-4k/) ([buy](https://www.apple.com/shop/buy-tv/apple-tv-4k))|$179/$199|4k@60|YES|10/DV|ax|1000M|YES|No|2nd gen, A12, 3GB/32-64GB, DV-5/8, DC:DTHD/DTSHD->PCM, PT:LS DA, BT 5.0
[Amazon Fire TV stick 4K MAX (2021)](https://www.amazon.com/dp/B08MQZXN1X) ([buy](https://www.amazon.com/dp/B08MQZXN1X))|$55|4K@60|YES|10/+/DV|Opt (9a)|YES|ax/Opt (8a)|V:Better A:Better|1st gen, AV1, DV-5/8, PT:LS DA, 1.8Ghz/2GB/8GB
[Amazon Fire TV stick 4K (2018)](https://www.amazon.com/all-new-fire-tv-stick-4k-with-alexa-voice-remote/dp/B08XVYZ1Y5) ([buy](https://www.amazon.com/all-new-fire-tv-stick-4k-with-alexa-voice-remote/dp/B08XVYZ1Y5))|$40|4K@60|YES|10/+/DV|dual ac 2x2|Opt (9a)|YES|Opt (8a)|1st gen, PT:LS DA, 1.7Ghz/1.5GB/8GB
[Amazon Fire TV stick Lite](https://www.amazon.com/dp/B091G4YP57) ([buy](https://www.amazon.com/dp/B091G4YP57))|$30|1080p|NO|10/+|ac/Opt (9a)|YES|Opt (8a)|V:Good A:Good|BT 5.0 LE, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[ChromeCast w/Google TV HD](https://store.google.com/product/chromecast_google_tv) ([buy](https://store.google.com/product/chromecast_google_tv))|$30|1080p|No|10/+|dual ac|Opt|YES|Opt (8a)|AV1, DC:DD+, PT:LS DA/DTS, S805X2, 1.5GB/8GB
**[ChromeCast w/Google TV 4k](https://store.google.com/product/chromecast_google_tv)** ([buy](https://store.google.com/config/chromecast_google_tv))|**$50**|4k@60|YES|10/+/DV|dual ac|Opt (9b)|YES|Opt (8a)|2nd gen. AV1, DV-5/8, DC:DD+, PT:LS DA/DTS, S905D3 1.9Ghz/2GB/8GB
-->

## What is the best client device to stream content to my TV?

The Amazon FireTV sticks, Roku and Google TV products all work very similarly at their respective price levels. Performance, interfaces, remotes all on par with each other with minor differences like types of buttons offered, apps supported, private listening, etc.. Limitations are similar as well; lack of USB storage and no lossless sound output is common across platforms. If you're just looking for something simple to plug into your TV and play Netflix/Hulu/Amazon Prime, $40 or so will get it done.  

Your choice may come down to a particular ecosystem you're already tied to or want to get into.  

If you use/want to use Amazon Alexa a lot you may want to go with a FireTV device.  

If you use/want to use Google Assistant a lot or want an Android TV experience, you may want to go with a Onn 4k Pro.  

If you want something ad-free, then an Apple TV 4K or an Onn 4k Pro + Projectivy/ATV Launcher.  

If you want something to just play files off a USB exfat drive with Kodi/VLC/etc.., then an Onn 4k Pro + Projectivy/ATV Launcher.  

If you want something more content provider-agnostic that searches across them well and has a lot of curated/free content, you may want to go with a Roku device.  

Once you start looking for advanced features, like external storage, gigabit ethernet, lossless audio or better performance for game streaming/emulation, you should start looking at pricier devices like the Nvidia Shield Pro, Fire TV Cube, Dune HD, and Odroid N2+  


## Can I watch live TV or record it and play it back on my HTPC?

**From an Antenna (OTA) or ClearQAM Cable (unencrypted):** 

Using an over-the-air (OTA) HD antenna avoids the "copy once" problem and most users are surprised by how much mainstream content they can get over the airwaves for free. Alternatively, with Cable, your provider may provide unencrypted ClearQAM channels, usually standard broadcast stations, without a cablecard. Even if you are not a cable TV subscriber, if the cable is connected to the providers network, they may still be sending ClearQAM programming into your home.  

If you use Plex Media Server, you can put a local pcie/usb tuner in your Plex server and set it up for Live TV and DVR, to be accessed by your preferred [Plex client](https://www.plex.tv/media-server-downloads/#plex-app). You can find a list of Plex compatible tuners [here](https://support.plex.tv/articles/225877427-supported-dvr-tuners-and-antennas/). The Live TV feature requires a Plex Pass ($$)  

If you can't or don't want to place the tuner at your server, you can use a networked tuner like a [HDHomerun](https://www.silicondust.com/) which you can find off ebay for cheap.  

If you don't have ethernet access, you can either use a wifi-capable tuner, like a [Tablo](https://www.tablotv.com) which is simpler to set up, or connect a [HDHomerun](https://www.silicondust.com/) to a [Ethernet->Wifi bridge](https://www.amazon.com/gp/product/B01N5RCZQH).  

For Antennas, stick to well-known brands like Channel Master, Antennas Direct, Winegard and Televés. For reception signal maps check [here](https://www.fcc.gov/media/engineering/dtvmaps), [here](https://www.antennasdirect.com/transmitter-locator.html) and [here](https://rabbitears.info/searchmap.php)  

If you don't want to use Plex to interface with your tuner, but want similar simplicity, you can install the [Channels](https://getchannels.com/) server/dvr somewhere ($$) (they support a range of PC-like hardware), point it to a networked [HDHomerun](https://www.silicondust.com/) (and ONLY HDHomerun) tuner with an antenna or your provider's [TVEverywhere](https://getchannels.com/tv-everywhere/) feed and then access it with the Channels client app.  

A more involved, but free, setup would be connecting a [tuner](https://linuxtv.org/wiki/index.php/ATSC_USB_devices) to a Raspberry PI 4 and using the TVHeadend backend ([included in the LibreElec OS](https://techlory.com/blog/2025/01/22/use-tvheadend-raspberry-pi-and-kodi-to-stream-tv-in-your-home/)) with tvhProxy to get the tuner into Plex. Again, if you don't want to use Plex, skip tvhProxy and simply use Kodi with the TVHeadend client on your frontends to access the TVHeadend backend. If you need to do video transcoding for your clients, replace the Pi with a used intel 7th gen+ PC off ebay.  

You can use MCEBuddy to remove commercials and convert your recorded programming to other file formats.  

For a more complete, albeit old, guide to setting up live TV with a generic TV tuner using ServerWMC and MediaBrowser, [see this post.](https://www.reddit.com/r/htpc/comments/2vc16r/guide_network_streaming_of_live_tv_access_tv/). You can use MCEBuddy remove commercials and convert your recorded programming to other file formats for use with PleX Media Server, Kodi or Mediabrowser.  

**From Cable (encrypted):** 

**NOTE: Cable Cards for encryption are becoming increasingly rare. You should eventually move to streaming from your Cable Service provider or a dedicated TV Streaming Service provider, in the next two options. Also, Windows 10+ will not include or support Windows Media Center or ServerWMC, but it will continue to work with older versions of Windows.**  

The most common solution was to use a Silicon Dust [HDHomerun Prime](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p4432023.m570.l1313&_nkw=hd+homerun+prime&_sacat=0) tuner, a Cable Card from your cable provider, and Windows Media Center software as the recording front-end. Presently, Windows Media Center is the only known way (using Windows) to record channels marked "copy once" by your cable provider. Different cable providers flag channels differently, and some flag *all* programming this way. Flagged content recorded by WMC can only be streamed to official WMC extenders, which are rare. But you can use ServerWMC to provide live TV to Kodi or MediaBrowser/Emby clients.  
If you only want to watch "copy once" channels, you can use the official HDHR app on Android, Xbox, Windows, etc..  
If you don't need "copy once" channel support, then your options are similar to the Antenna section above, albeit your tuner still being the HDHomerun Prime. That is, adding your tuner into a [Plex Media Server](https://www.plex.tv) or into a [Channels](https://getchannels.com) server and using their respectively client apps, or accessed directly with Kodi/Mediabrowser and its [add-on](https://kodi.wiki/view/Add-on:HDHomeRun).  

**From Cable Service (over the internet):** 

If you don't want to or can't use a tuner with an antenna or cable connection, some TV providers will allow you to pull TV programming over the internet.  

To do this, you need your normal cable subscription service, a login to your provider and a client/server program. The easiest way to currently do this is to install the [Channels DVR Server](https://getchannels.com/dvr-server) ($$) software somewhere on your network, configure it to use the [TV Everywhere](https://getchannels.com/tv-everywhere/) feature, with your provider and login credentials and then use the [Channels](https://getchannels.com/apps) client software on your devices to access the channels. On a PC client this can be done either through the server's web ui or via Kodi with the [Channels DVR](https://kodi.wiki/view/Add-on:Channels_DVR) plugin.  

**From Streaming Service (over the internet):** 

Youtube TV, Fubo, DirectTV Stream, or Hulu Live TV  on the premium end. Philo or Sling TV on the low-end. It depends on the [channels you want](https://www.google.com/search?q=youtube+tv+directv+hulu+fubo+sling+philo&tbs=qdr:m). Fubo tends to have the most channels/packages.  


**From your own media content:**

If you want to make virtual TV channels out of your own content, look at [ersatztv](https://ersatztv.org) in combination with either a Plex/Jellyfin/Channels DVR-type server or directly with clients like VLC or TiviMate through m3u playlist files.  

## Can I stream/how do I serve my content from another computer or a networked storage device?

Figure out how many clients you will be serving to simultaneously and what types of clients (local or remote). Assume you will be transcoding content for at least 1/3 of the clients (unless you know otherwise). So, for example, if you determine you will have 3 simultaneous clients, assume 1 of them will be transcoding, so choose a server with hardware that can do at least 1 transcode.

Look at the [Sample Builds](/wiki/sample-builds#nasmedia-server-builds) page for pre-built and DiY media server solutions based on that. You can buy a very capable media server for under $200. Don't forget to take into account the amount of storage you need, which can be signifigant, whether it be [internal, external, or networked with a NAS](/wiki/storage). Ripped/Remux 1080p movies can reach 25GB in size EACH, with 4k ones up to 4x that. Your storage can be separate with a pre-built NAS, or built into the media server, depending on your technical ability.  

Once you have the hardware you need, connect the media server and/or NAS to your router over ethernet, attach and/or mount the internal/external storage to the server, install and configure [media server software](/wiki/video#video-software), then install the server's player software on your [media client](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) devices, making sure they're compatible with the codecs you want to play.  

[Media serving software](/wiki/video#video-software) can be PleX Media Server or something similar like Emby/Jellyfin. The advantage of these media servers is that they can transcode the files in real time to meet the needs of your target client device (HTPC, phone, tablet, smart tv, remote client, etc.) and organize your media with metadata. It will serve the media to your client devices or HTPCs using the software's respective client app, over the network. Make sure your network that is serving the clients has bandwidth sufficient to do this. Ideally the clients should be on 100 Mbps ethernet for 1080p content or 1 Gbps ethernet for 4k content. If you're attempting to use wifi instead, make sure the client's bandwidth (via a speed test) is greater than that of your [content's bitrate](https://mediaarea.net/en/MediaInfo). Running these on Linux or a dedicated OS (like Unraid/TrueNAS/OMV) provides the most capabilities (esp. for gpu transcoding), but Windows is also possible.  
  
If you don't want to use media serving softwares, or you don't need real time transcoding, you can simply share your content storage out using a [network samba share](https://www.net-usb.com/share-hard-drive-over-network/#usb), whether that be configured in windows or linux, or connected to a router with a USB port. You can then access the network samba share on your [media clients](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc), and use normal media players like Kodi, MPC-BE, etc.. to play the content. For those instances where you can't use one of these media players (to access network samba shares), try a DLNA server and client.  



## How do I add Network Attached Storage (NAS) to my network for my HTPC/media devices?

[See our separate wiki page here](/wiki/storage)  

## What resolution and audio is supported on streaming service X?

The max resolution and audio supported by a particular service on a traditional HTPC varies by the service, OS and program (browser/app) used.  

**Make sure to configure your system/browser first via the setup sections of the [Audio](/wiki/audio#application-specific-setup-for-bitstreaming) and [Video](/wiki/video#application-specific-setup-for-hardware-decoding) wiki pages**. For better video, audio and HDR support, use a media device instead.  

The following are the current capabilities of the major streaming services as we know them on a PC. Anything 4K will require [HDMI 2.0 and HDCP 2.2](/wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility) support. These are always subject to change, both for the better and for the worse. If you have any contradicting data, please let us know.  

- [NETFLIX](https://help.netflix.com/en/node/30081)  

  - *Windows:* (MS Edge/MS Store App) [4k HDR10](/wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility), [DD+ 5.1 Atmos](https://help.netflix.com/en/node/14163). (Chrome/Firefox) 1080p SDR Stereo
  - *Linux:* (Opera) 1080p SDR, (Other Browsers) 720p SDR

- [AMAZON PRIME VIDEO](https://www.amazon.com/gp/help/customer/display.html/ref=hp_left_v4_sib?ie=UTF8&nodeId=GUVGB3QMQRYRERYW)  

  - *Windows:* (App/MS Edge/Safari) 1080p SDR, (Chrome/Firefox) 720p SDR. Stereo
  - *Linux:* 480p SDR, Stereo

- [HULU](https://help.hulu.com/s/article/video-quality?language=en_US)  

  - *Windows:* (MS Store App w/Edge browser as default) 720p SDR, DD+ 5.1. (Browser) 720p SDR, Stereo.
  - *Linux:* 480p SDR, Stereo
 
- [YOUTUBE](https://support.google.com/youtube/answer/78358?hl=en#:~:text=To%20watch%20YouTube%20videos%2C%20make,Internet%20connection%20with%20500%2B%20Kbps)  

  - *Windows:* 4k HDR10, Stereo
  - *Linux:* 4k SDR, Stereo

- [YOUTUBE TV](https://support.google.com/youtubetv/answer/7129767?hl=en&co=GENIE.Platform%3DDesktop#zippy=%2Cmobile-devices-computers%2Cstreaming-media-players-smart-tvs-game-consoles)  

  - *Windows:* 1080p SDR, Stereo
  - *Linux:* 720p SDR, Stereo

- [HBO MAX](https://help.hbomax.com/US/Answer/Detail/000002506)  

  - *Windows:* (MS Edge/Safari/Chrome/Firefox) 720p SDR. Stereo
  - *Linux:* (Chrome/Firefox) 720p SDR?

- [DISNEY+](https://help.disneyplus.com/article/disneyplus-computer-browser-requirements)  

  - *Windows:* (App) 720p SDR DD 5.1. (MS Edge) 720p SDR, (Chrome) 720p SDR, (Firefox) 480p SDR. Stereo.
  - *Linux:* (Chrome/Firefox): 480p SDR, Stereo

- [APPLE TV](https://support.apple.com/guide/tvplus/welcome/web)  

  - *Windows:* (MS Edge/MS Store App) 4k HDR10 DD+ 5.1 Atmos. (Chrome/Firefox) 720p SDR
  - *Linux:* Unknown, but will not be higher than 1080p

- [TWITCH](https://help.twitch.tv/)  

  - *Windows:* 1080p SDR?
  - *Linux:* 1080p SDR?

- [SPOTIFY](https://support.spotify.com/us/article/audio-quality/)

  - *Windows:* (App): w/Premium: 24-bit/44.1 kHz FLAC, wo/Premium: AAC 160 Kbps. (Web) w/Premium: AAC 256 Kbps. wo/Premium: AAC 128 Kbps

- [VUDU](https://support.vudu.com/en_us/categories/general-requirements-r1VPwDURP)  

  - *Windows:* (Browser/App) 1080p, Stereo
  - *Linux:* Not supported, use Movies Anywhere for limited support

- [PEACOCK TV](https://www.peacocktv.com/help/article/what-devices-and-platforms-are-supported-by-peacock)  

  - *Windows:* (Edge) 1080p? SDR, AAC Stereo
  - *Linux:* Not supported

- [PARAMOUNT+](https://help.paramountplus.com/s/article/PD-Supported-Devices)  

  - *Windows:* Unknown, but will not be higher than 1080p
  - *Linux:* (Chrome/Firefox) 576p SDR, Stereo?

- [DISCOVERY+](https://help.discoveryplus.com/hc/en-us/articles/1500000101182-Browsers-and-devices-supported-by-discovery-)  

  - *Windows:* Unknown, but will not be higher than 1080p
  - *Linux:* Unknown, but will not be higher than 1080p

## How can i play my DVD/Blu-ray discs on my HTPC?

[See our separate wiki page here](/wiki/video#how-can-i-play-my-dvdblu-ray-discs-on-my-htpc)

## How can i rip my DVD/Blu-ray discs and what are some good quality settings to use?

For DVDs and regular HD blu-ray any optical drive that can read the discs will do, internal or external, and you can spend <= $75 on one. For UHD discs, you should have a UHD or UHD-Friendly compatible drive with locked-in firmware. Check our [optical drives section](/wiki/components#optical-drives).  

You will then use software to rip the content off the disc. It's recommended to do this process in two stages, especially if you need content re-encoded for compatibility or space-saving..  

First, use the [MakeMKV](http://www.makemkv.com/) program to extract the content off the disc. You can choose all the video/audio titles on the disc, just some of them, or just the main one. In the end, this will make a full quality MKV file without changing the format or size of the content. This isn't CPU heavy and can be done on a very minimal system.  
If you want to make a full ISO instead of an MKV, click the Backup icon in the toolbar to output the disc to (*DVD*: an ISO file; *Blu-Ray*: a folder, then make an ISO of the folder using [ImgBurn](https://www.imgburn.com/index.php?act=download)).  

If you're after the best quality, you're done. Play the file with your [favorite media player](/wiki/video#video-software) or put the file on your [media server storage for serving](/wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device).  

However, these full quality files are large. DVDs can be up to 9.9GB (11 Mbps), FHD Blu-rays 36GB (40 Mbps), and UHD Blu-Ray 115GB (128 Mbps) for 2 hours worth of content. For this reason, some people move to stage two next and use a program called Handbrake to make the files smaller while giving up on some visual quality. It's up to you.  

[Handbrake](https://handbrake.fr/) is used to re-encode content for size, bandwidth and/or compatibility. The goal is to create a file that is highly compatible with client devices and is reasonable on bandwidth use, but doesn't negatively effect the video quality. Re-encoding can take a long time, depending on how fast your CPU is; a modern 4-6 core CPU is ideal, but if you don't care about how long it takes, then it doesn't matter. You can also use a iGPU/dGPU for faster encoding times. Intel QSV (QuickSync) and Nvidia NVENC encoders are supported, but while you reduce encoding times, you also reduce visual quality a bit as GPUs aren't as good encoding as CPUs.  

In Handbrake..  

Open the content file and on the Summary tab, choose MPEG-4 (MP4) or Matroska (MKV) for the output Format. Neither changes the file size. MP4 is compatible with more devices, but MKV has better embedded subtitle and multi-track audio support. If you're using subtitles and want to embed them into the file, use MKV.  

On the Dimensions tab, if you want to downscale to a different resolution, use Resolution Limit.  

On the Video tab:  

- Video Encoder: H.264 8-bit codec, for best client compatibility decoding. Alternatively, the H.265 10-bit codec is also possible and will yield better compression on >= 1080p content, but if you have old clients (pre-2016), decoding could be a problem. If old clients aren't an issue, choose the H.264 option for DVDs and H.265 for blu-rays.  

- Framerate : Same as Source, Constant Framerate  

- Encoder Options: Preset: Medium, Level: 4.1 (H.264), Level: 5.1 (H.265)  

- Quality: Constant Quality is the more efficient encoding method. Use 19 RF (DVD) or 18 RF (1080p/4K Blu-Ray). Use 20-22 if you're really tight on disk space. If you need to hit a target file size, then use Avg Bitrate instead, but you should target bitrates of >= 1500 kbps (DVD), >= 3000 (720p), >= 7000 (1080p), >= 25000 (4K).  

On the Audio tab, the default is to convert the audio track to a highly compatible AAC, stereo track. If you want to preserve HD audio from your content, you should set the track shown to Passthru instead. Optionally, add (under Tracks) an additional AAC (FDK)/Stereo audio track for client compatibility.  

A lot of these settings are subjective, especially video and audio quality. Play around with the settings until you find ones that meet your requirements for a balance between visual/audio quality, disk space and encoding time. Use [MediaInfo](https://mediaarea.net/en/MediaInfo) to check your output file's info.  

For a more automated way to do this process, look at [Automatic Ripping Machine](https://github.com/automatic-ripping-machine/automatic-ripping-machine)  

Example encode:  
- Source: **400MB** - 4K - 53.6Mbps - H.265 10-bit - DTS-HD MA
  - Destination @ H.265 10-bit, RF 18, audio passthru: **208MB**, 28.2Mbps (52% of original size)  
  - Destination @ H.265 10-bit, RF 20, audio passthru: **154MB**, 20.9Mbps (38.5%)  
  - Destination @ H.264, RF 18, audio passthru: **285MB**, 38.5Mbps (71.1%)  
  - Destination @ H.264, RF 20, audio passthru: **203MB**, 27.4Mbps (50.7%)  

## What do I need for 4k ultraHD compatibility?

**If you want to use a pre-built HTPC/media device**

See the top of our [Sample Builds](/wiki/sample-builds#htpc-pre-builtsmini-pcs) wiki page or our table of media devices [above](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc).  

**If you're building a traditional DiY HTPC**

*Short version:*

See the DiY section of our [Sample Builds](/wiki/sample-builds#htpc-diy-builds) wiki page. 

4k local content: [HDMI 2.0 motherboard](/wiki/hdmi20) (1.4 if only 30fps non-HDR) + >= [Intel 7th Gen/Gemini Lake/Athlon 200GE/Ryzen 2200G CPU](/wiki/components#cpus) **OR** CPU (>= circa 2008) + dGPU >= [Nvidia GT1030/AMD RX 550/5x00](/wiki/components#gpusgraphics) **(REC: Ryzen 5500GT+B550 mobo)**.  

4k youtube: [HDMI 2.0 motherboard](/wiki/hdmi20) + >= [Intel 7th Gen/Gemini Lake/Athlon 200GE/Ryzen 2200G CPU](/wiki/components#cpus) **OR** CPU (>= circa 2008) + dGPU >= [Nvidia GT1030 GDDR5/AMD RX 5x00](/wiki/components#gpusgraphics) **(REC: Ryzen 5500GT+B550 mobo)**.  

4k netflix: HDCP 2.2 display(s), [HDMI 2.0 motherboard](/wiki/hdmi20) + >= [Ryzen 3200G/3400G/Intel 7th Gen/Gemini Lake CPU](/wiki/components#cpus) **OR** CPU (>= circa 2008) + dGPU >= [Nvidia GTX 1050 3GB/AMD RX 550/5x00](/wiki/components#gpusgraphics) **(REC: Ryzen 5500GT+B550 mobo)**. Windows 10+. Microsoft [HEVC Video Extensions](https://www.microsoft.com/en-us/p/hevc-video-extensions/9nmzlz57r3t7). Netflix app/Microsoft Edge browser. Intel MEI driver/ME firmware (Intel iGPU). Netflix [Premium Plan](https://help.netflix.com/en/node/24926). Netflix [Test Patterns](https://www.netflix.com/title/80018499).  

4k/UHD Blu-Ray disc playing: HDCP 2.2 display, [HDMI 2.0 motherboard w/SGX support](/wiki/hdmi20), [Intel i3/5/7/9](/wiki/components#cpus) **7th-10th Gen CPU w/iGPU ONLY** **(REC: Intel i5-8xxx+Gigabyte H370N mobo)**. Windows 10+. Use of a dedicated GPU (dGPU) is **not** supported.  

4k@120Hz: See [Wiki:Video:What options are there for 4k @ 120 Hz video output?](/wiki/video#what-options-are-there-for-4k--120-hz-video-output)  

*Long version:*

**MAIN REQUIREMENTS**

The major requirements for full 4k compatibility are HDMI 2.0a, HDCP 2.2, hardware HEVC decoding (and support for Intel SGX in the bios if playing UHD blu-ray discs). Anything less will be a limited and incomplete implementation of the upcoming standards.

**HARDWARE**

Virtually all modern CPUs with integrated graphics can display 4k video. BUT, all of the components in your home theater (TV, AV Receiver and HTPC motherboard) will need to have a HDMI 2.0a port in order to use all sources of 4K content.  
On the AMD side, this starts with the Ryzen 2200G and on with any supported motherboard. Buy a Ryzen 5500GT and B550 motherboard and move on.    
On the Intel side, this started with 7th gen (7xxx) CPUs, but required a [special hdmi 2.0 motherboard](/wiki/hdmi20); But since 11th gen (11xxx) CPUs, any supported motherboard will work. Buy a i3-13100 and B760 motherboard and move on.

If one of the motherboards doesn't fit what you need, or you are upgrading an older, existing system that lacks the above, you can choose a [dedicated GPU](/wiki/components#gpusgraphics) to add on to your system that has these features. The Intel Arc A380 is popular, as is the RX 6400 on the AMD side.

You CAN display 4k video at 30hz via older HDMI 1.4 and 4k video at 60hz via a Displayport 1.2 connection but you will run into other problems. HDMI 1.4 won't support HDCP 2.2/4k blu-ray/Netflix and the Displayport 1.2 connection won't display HDR content, so stick to the more modern iGPUs/dGPUs above.

**DRM**

If you plan on playing DRM protected content, for instance 4k netflix, you will need to have a HDMI 2.0 port that supports HDCP 2.2 or a Displayport with an active DP 1.x->HDMI 2.0 adapter. This can take the form of an AMD Ryzen 3200G+ CPU with supported mobo **OR** Intel 7th-14th Gen CPU and [supported motherboard](/wiki/hdmi20) **OR** Any CPU and an add-on dGPU, **only** Nvidia >= GTX 1050 3GB, AMD >= RX 4xx/5xx/5x00/6x00, or Intel >= ARC A310.  
With pre-builts, like Mini PCs, HDCP 2.2 is **NOT** a given with HDMI 2.0, so either stick to DiY, use one that specifically mentions it, or use the recommended pre-built solutions from our builds page.

If you plan on playing UHD Blu-ray discs, things are even more restrictive; you are further limited to Intel CPUs w/SGX support (Intel i3/5/7/9 7th-10th Gen **ONLY**) + a [HDMI 2.0 motherboard w/SGX support](/wiki/hdmi20). Dedicated GPUs are **NOT** supported. **We do not recommend this** and you should play rips or ISOs of your discs. See our wiki section [here](/wiki/video#how-can-i-play-my-dvdblu-ray-discs-on-my-htpc). 

To test for HDCP 2.2 compliance, use [Cyberlink Ultra HD Blu-Ray Advisor](https://www.cyberlink.com/prog/bd-support/diagnosis.do) or [Corel Ultra HD Blu-Ray Check Tool](https://dwnld.windvdpro.com/tools/CorelUltraHDBlurayCheckTool.exe)  

**SOFTWARE/CONTENT**

The only 4k content supported on a PC are: Local files, UHD blu-ray discs, Youtube and Netflix. See the [section above](/wiki/faq#what-resolution-and-audio-is-supported-on-streaming-service-x) on what resolutions are supported for other services and our [software section](/wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) for players. 

If you want access to more 4k content, on your favorite streaming services, use a [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead.  

It is highly likely that the 4K content will be encoded in the H.265 (HEVC) codec, the successor to H.264. Hardware decoding of H.265 is limited to:

- [Intel 7th-14th Gen/Apollo/Gemini Lake CPU w/iGPU](/wiki/components#cpus) 

- [AMD >= Athlon 2x0GE/3000G, >= Ryzen 3 2x00G CPUs](/wiki/components#cpus) 

- [Nvidia >= GTX 10xx, AMD >= RX 550/5x00/6x00, Intel ARC](/wiki/components#gpusgraphics) dGPUs 

All options are sufficient, and have benchmarked playing 4K 400Mbps bitrate videos at >= 70fps ([See Here](https://forum.doom9.org/showthread.php?p=1803012#post1803012)). Most 4K videos encoded in HEVC have avg. bitrates between 15-128Mbps (Netflix 4K is HEVC encoded at 16Mbps).

HDR is also a popular feature these days. For additional requirements, see the section below.

**COST**

If you go the CPU w/IGPU route, you can expect to spend about $125 for a CPU (like a Intel i3-13100 or AMD Ryzen 5500GT) and between $90-$150 for a Intel B760/AMD B550 motherboard, respectively, depending on the form factor.  

If you go the dedicated GPU route, an Intel ARC A380 will cost around $100, while a AMD RX 6400 will cost around $140.  

With either option, expect to spend more than $450 on a complete new build. You can get away with less if you get a used SFF system off ebay and add one of the low profile dedicated GPUs. See the Sample Builds wiki page.  

If you are unsure what to get for your particular requirements, ask us and we will steer you in the right direction.  


## What is HDR video and what do I need to take advantage of it?

HDR stands for High Dynamic Range. It's a technology used to produce better looking video by preserving details in the darkest and lightest portions of a frame resulting in better contrast. Common standards are HDR10, HDR10+ and Dolby Vision. [See here](/wiki/video#video-metadatacolor-technologies) for the gory technology details. 

For a HTPC, this means HDR support must be in the video, GPU, video interface (HDMI/DP) and ultimately your output device (typically a TV).  

HDR10 is supported on HTPCs under Windows, macOS Catalina, Android and (usually) libreelec/coreelec operating systems. Linux is NOT supported.  

**DOLBY VISION AND HDR10+ MEDIA PASSTHROUGH IS NOT SUPPORTED ON HTPCS**; If you need support for these, you'll need a [media device/non-PC](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc), like a Nvidia Shield, Fire TV, Dune HD, etc..  

HDR streaming content is limited thus far and only found on Netflix and Youtube services for a PC. If you want access to more HDR content on your favorite streaming services, use a [media device](/wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead.  

For setting up HDR on your client, [See our separate wiki page here](/wiki/hdr)  

That all being said, HDR is supported on a PC with at least HDMI 2.0a or DisplayPort 1.4 ports. 

If you're not comfortable building DiY, look at the pre-built recommendations at the top of the [Sample Builds](/wiki/sample-builds) page.  

Otherwise, if you stick to Ryzen APUs or Intel >= 11th gen CPUs below, any paired motherboard will have the HDMI port you need.  

The following CPU iGPUs/APUs are officially supported:  

- Intel 7th+ Gen (7xxx+) Core i3/i5/i7/i9/Ultra, Intel >= 12th gen (G6900/G7400) Celeron/Pentium, Intel N5xxx/N6xxx Jasper Lake. **(REC: Intel i3-13100+B760 mobo)**  

- AMD >= Ryzen 3 2x00G APU, >= Athlon 2x0GE/3000G **(REC: Ryzen 5500GT+B550 mobo)**

It's also available on the following dGPUs: Nvidia GTX >= 950, GT >= 1030, Titan X, Quadro P5000/P6000, AMD RX >= 4x0/5x0/5x00, Radeon 7, Vega 56/64, Intel ARC >= A310.  

For older DiY motherboard support, reference our [HDMI 2.0 motherboards](/wiki/hdmi20) page.  

## Should I buy a low-power version of a CPU?  

*This section applies to DiY*  
CPUs use power, sometimes more than you want. This power usage produces heat, which makes your fans work harder and sound louder to keep the CPU temperature under control. This number is the TDP and is in watts.  
CPU mfgrs like Intel and AMD sometimes make low-power versions of their CPUs with a lower TDP.  
Intel makes 65W and 35W versions of their i3 CPUs, with the 35W version having a "T" suffix (e.g. i3-13100T vs i3-13100) with a signifigantly lower Base Frequency to stay within the 35W limit.  
AMD makes 65W and 35W versions of their APUs, with the 35W verion have a "E" suffix (e.g. 3400GE vs 3400G) with a signifigantly lower Base Frequency to stay within the 35W limit.  

Usually, the low-power models are more expensive and limited in availablility, therefore harder to find.  
It's better to just buy the normal power version and lower the Frequencies and/or TDP yourself using available methods.  
This tends to be easier on AMD as they have a 45W profile you can choose for 65W APUs and you can also underclock the frequencies without restriction.  
Intel has options as well for their CPUs, they're just less varied or more restrictive.  

Here are the methods you can use:  
 
 Intel  
  1. In Windows (OS): Control Panel->Power Options->Power Plan->Change advanced..->Processor Power Management->Maximum processor state->Lower percentage from 100%  
  2. In Windows (Intel): Install the Intel Extreme Tuning Utility app. Lower Base/Boost CPU frequency or TDP.  
  3. In BIOS: Depends on motherboard vendor. Lower PL1 and PL2 power limits to the max watts you want to pull (e.g. 35W).  
  4. Fan control: Lower the max RPM on your fans causing CPU to throttle its frequencies when hitting thermal limits. Viable, but NOT recommended.

 AMD  
  1. In Windows (OS): Control Panel->Power Options->Power Plan->Change advanced..->Processor Power Management->Maximum processor state->Lower percentage from 100%  
  2. In Windows (AMD): Install the AMD Ryzen Master app. [Lower Base/Boost CPU frequency/TDP or Activate ECO mode](https://www.amd.com/system/files/documents/ryzen-master-quick-reference-guide.pdf). In Mini PCs, use [Universal x86 Tuning Utility](https://amdaputuningutility.com/) to lower the max TDP.  
  3. In BIOS: Depends on motherboard vendor. Look in the CBS/NBIO/System Config menus to lower the TDP.  
  4. In BIOS: Depends on motherboard vendor. Lower the base/boost cpu frequencies.  
  5. Fan control: Lower the max RPM on your fans causing CPU to throttle its frequencies when hitting thermal limits. Viable, but NOT recommended.  

## How do I set up audio/video on my HTPC?

Audio: [See our separate wiki page here](/wiki/audio)  

Video: [See our separate wiki page here](/wiki/video)  


## Do you have any sample builds I can refer to?

[See our separate wiki page here](/wiki/sample-builds)

## How can I set up an HTPC for the elderly/disabled?

**THIS QUESTION IS UNDER CONSTRUCTION!**  

If you just need streaming services and automation isn't needed, then a Roku is usually the easiest solution. If you need local playback in addition to this, an Onn 4k Plus frontned with Kodi/Plex/Jellyfin software with a N100 mini pc backend connected to USB storage is best.  

But if internet is not available, you have poor network conditions and/or automation is desired, this lends itself well to HTPCs, especially under x86 hardware 
with linux, windows, or especially hardware that supports installing [Libreelec](https://libreelec.tv/downloads/) (like Raspberry Pis and cheap [mini pcs](/wiki/sample-builds#htpc-pre-builtsmini-pcs)) so you can boot directly into Kodi  

Some options/considerations for this are:  

1. Use Linux/Windows for OS
   - Simple: Install Kodi, Plex HTPC, etc..; set to run on boot, configure.
   - Advanced: If you need to run multiple programs, use a launcher on boot, like Flex Launcher or just map remote keys to each app with AutoHotKey (see below).
3. Use [Libreelec](https://libreelec.tv/downloads/)/CoreElec for OS on compatible hardware
   - Boots into a Kodi interface
   - Configure Kodi to your liking 
5. A simple remote.
   - RF: [OSMC](https://osmc.tv/store/product/osmc-remote-control/), [FM4](https://www.amazon.com/Seleven-Universal-Control-Wireless-Android/dp/B01FVUGPE8), [G20S](https://www.amazon.com/WeChip-G20-Control-Wireless-Sensing/dp/B07P322VRP)
   - IR: [WeChip W3](https://www.amazon.com/WeChip-W3-Wireless-Control-Projector/dp/B09XMF5YN1), [Argon IR](https://www.amazon.com/Argon-Raspberry-Infrared-Batteries-Included/dp/B091F3XSF6) w/FLIRC or rPI 4+Argon ONE case
   - [FLIRC](https://flirc.tv/products/flirc-usb-receiver?variant=43513067569384) w/any IR TV/MCE remote. (e.g. [OneForAll Streamer](https://www.oneforall.com/universal-remotes/urc7935-streamer-remote))
   - Controller: 8bitdo Ultimate 2c w/Controller Companion for button mapping

Notes:
 - Common: Start on boot
   - Put program shortcut in startup folder (Windows: %appdata%\Microsoft\Windows\Start Menu\Programs\Startup, [Linux](https://kodi.wiki/view/HOW-TO:Autostart_Kodi_for_Linux))
   - If you need to run the program with command line options/switches, create a <program>.bat file containing what you want to run and put that in the startup folder
 - Common: Key/Button mapping
   - Some programs have a built-in feature for mapping keys to functions like Kodi's [keymap](https://kodi.wiki/view/Keymap) and Plex's [inputmaps](https://support.plex.tv/articles/plex-htpc-input-maps/). If not, use the AutoHotKey (AHK) program to do this; it has a more advanced feature-set.
   - If not mapping a normal key, get its "scancode" by either using [KeyboardStateView](https://www.nirsoft.net/utils/keyboard_state_view.html), or by opening the window of a running .AHK script and using Cntrl+K. You can then use this in your AHK script/inputmap to do basically anything, open a program, etc...
   - Controller Companion if using a controller.
 - Common: Remote Access for help
   - Linux/Windows: Teamviewer, Rustdesk, Chrome Remote Desktop
   - Libreelec: VPN to network (@router or @device w/tailscale) + VNC
 - Common: Power Control
   - Plug device into a [smart power plug](https://www.amazon.com/Assistant-Controlled-Google-Enabled-Vacation/dp/B07XZT24B8), control power on/off by mobile app or cheap ECho Pop, set HTPC after power loss behavior in BIOS
 - Kodi
   - Starting in Full Screen (Settings->System->Display->Expert->Display mode)
   - Starting up in certain libraries (Settings->Appearance->Home)
   - [Removing unneeded skin features/libraries](https://kodi.wiki/view/Add-on:Estuary/Settings#Main_Menu_Items_Settings)
   - [Changing a library view type](https://kodi.wiki/view/Basic_controls#Sideblade_Menu)
   - [Creating smart playlists](https://kodi.wiki/view/Smart_playlists)
   - Have Kodi autoplay smart playlists on startup with ````<onload>```` and ````PlayMedia()```` [in a skin's Startup.xml and guisettings.xml](https://forum.kodi.tv/showthread.php?tid=53092)
   - [Have Kodi autoplay certain playlists on a schedule](https://forum.libreelec.tv/thread/1458-automated-video-playlist-using-time-schedules-w-auto-volume-control/)
 - VLC
   - Loop playlists on start with options like: ````--fullscreen --loop --playlist-autostart --playlist-tree <path>````
 - Plex HTPC
   - [Key/Button mapping](https://support.plex.tv/articles/plex-htpc-input-maps/) through a inputmaps json file. Can map to plex functions and even shutdown/reboot for host system. Keys can be the actual keys or scancodes. Supports remote and game controllers
 - [MediaPortal](https://www.team-mediaportal.com/)

<!-- Footer -->
&nbsp;

---

*This page was last updated on 2026-01-25*

