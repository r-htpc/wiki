# FAQ

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

*This page is best viewed with a PC web browser.*  

<!-- Section -->

## What is a HTPC?

HTPC stands for Home Theater Personal Computer.

Traditionally a HTPC is a PC with a purpose to play and/or serve media in a theater-type setting (living room, etc..). It does this through specific hardware and/or software. 

Specific hardware can be a TV tuner card, high-end sound card, other decoder cards, remotes or a case optimized for noise and/or space.

[Specific software can be media players, codecs, certain operating systems and specialized media software interfaces](/htpc-wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up).

Media can be video content from [ripped personal discs](/htpc-wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use), [streaming services](/htpc-wiki/faq#can-i-use-my-htpc-for-streaming-from-services-such-as-netflix-amazon-hulu-etc), audio, photos, or emulation gaming content.  

As computing power has gotten smaller and smaller, traditional PCs have given way to integrated media devices which have blurred the line over what a PC is.

A media device such as a Roku player is very small and performs most of the functions a PC does, with CPU, memory, storage, operating system, etc.. The biggest distinction is that [these devices](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) are usually designed specifically for playing media in a Home Theater setting.

MOST of these small devices simply act as clients (they may not even connect to a server in your setup, but simply to internet streaming services, like Netflix), 
but a small, powerful few also can act as servers.

An example would be the Nvidia Shield TV. It is a powerful integrated device with an android media interface when connected to a TV. It also can have storage on it which allows you to install server software (like Plex for example) and serve media to other clients in your home.

This can be confusing; it's not a traditional HTPC per-se, but performs the functions of one.

Below we'll advise you on how to get started with a HTPC.

What is NOT a HTPC: Playing media just on your laptop. Playing media at your desk. Playing media on a computer monitor(s).

<!-- Section -->

## How do I get started with a HTPC setup?

A HTPC whether it be a PC or media device, can act as a client, a server, both or standalone.  

For instance, it can act standalone and play media from [internal storage](/htpc-wiki/storage) or [streaming services](/htpc-wiki/faq#can-i-use-my-htpc-for-streaming-from-services-such-as-netflix-amazon-hulu-etc) to a connected TV/sound system.  

It can be a client connected to a TV/sound system and then [connect to a server](/htpc-wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device) which provides it the media to play.  

It can be a server which provides the media to the client as fore-mentioned.  

It can be client and server as well; connected to a TV as a client, playing internal media, but also has [server software](/htpc-wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) installed, which it uses to [send media to 
other clients in the home](/htpc-wiki/faq#can-i-streamhow-do-i-serve-my-content-from-another-computer-or-a-networked-storage-device).

You should first decide which of these roles you need based on your use-case, budget, and hardware available.  

You should reference the [video](/htpc-wiki/video)/[audio](/htpc-wiki/audio)/[storage](/htpc-wiki/storage) sections of the wiki as a guide to overall concepts if you're not familiar with them while researching a solution.  

A simple setup may just have a standalone PC (pre-built or DiY) with the [appropriate software](/htpc-wiki/faq#what-software-will-i-need-and-how-do-i-set-it-up) 
or a [media device](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc). Usually if streaming or a remote-based interface is a priority, then a media device is best, where a PC is better for more customization, 
keyboard/mouse interaction or lots of storage.  

An advanced setup with might have a server/storage tucked away somewhere and one or more client PCs/media devices connected to each display.  

Setups vary and there are many ways to do things. Finding the best way for you takes some time and research.  

In the next section are listed some quick-fire pre-built solution recommendations for client and server hardware based on common use-cases, with DiY [components](/htpc-wiki/faq#what-hardware-should-i-choose-for-my-htpc) and special scenarios further below. Detailed, complete PC solutions can be found in the [Building/Buying](/htpc-wiki/sample-builds) page of the Wiki. 

Once you build/buy your solution, you can then follow the setup in the appropriate sections of the video/audio/storage pages of the Wiki mentioned above to connect and configure the individual pieces.  

<!-- Section -->

## I want a HTPC/media device recommendation, but don't want to get into the complicated details

Here are recommendations for the most common scenarios, if you don't want to read our whole wiki and/or build something..

Streaming services only, no HD audio: Fire TV 4K stick (Amazon ecosystem) ($40), Chromecast w/Google TV (Google ecosystem) ($50)  

Streaming services only, HD audio: Nvidia Shield Tube ($150)  

Streaming services + 4K local content (high bitrate w/great > 200Mbps wifi), no HD audio: Fire TV 4K Max stick ($55), Chromecast w/Google TV 4k (Google ecosystem) ($50)  

Streaming services + 4K local content (high bitrate w/poor <= 200Mbps wifi), no HD audio: Fire TV 4K Max stick+[USB Ethernet adapter](https://www.amazon.com/Cable-Matters-Streaming-Including-Chromecast/dp/B07N2ZHFY9) ($65), Xiaomi Mi Box S+[USB Ethernet Adapter](https://www.amazon.com/UGREEN-Network-Ethernet-Supports-Nintendo/dp/B00MYTSN18) ($75)  

Streaming services + 4K local content, HD audio: Nvidia Shield Pro ($200)  

4K local content, HD audio: Odroid [C4](https://www.hardkernel.com/shop/odroid-c4/)/[N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ($65/$80) + CoreELEC  

Cheap Emulation Gaming: Odroid [N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ($80) + EmuElec/Batocera OR Used: >= 
[SFF/USFF PC - CPU >= i5-7500T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=\(hp%2Cdell%2Clenovo\)+\(i5-7500%2Ci5-8400\)+\(sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini\)+ssd&_sacat=179&LH_BIN=1&LH_TitleDesc=0&_sop=15&_udhi=175&LH_ItemCondition=2010%7C2020%7C3000) ($75)

1080p Casual Gaming: HP pre-built - [Ryzen 5600g/2x4GB RAM/>=256GB](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=hp+%285600g%2C5700g%29&_sacat=179&LH_TitleDesc=0&_odkw=hp+5700g&_osacat=179&LH_BIN=1&_sop=15) ($400-$500)

Single Layer Dolby Vision, HD audio: Nvidia Shield Pro ($200)  

1080p local content, HD audio: [ROCK64-2GB](https://pine64.com/product/rock64-2gb-single-board-computer/) / [Odroid XU4](https://www.hardkernel.com/shop/odroid-xu4-special-price/) / [Orange Pi 3 LTS 2GB](https://www.aliexpress.us/item/3256804169070057.html) ($45)  

1080p local content + Web Browsing (minimal), Linux: [ROCK64-4GB](https://pine64.com/product/rock64-4gb-single-board-computer/) / [Odroid XU4](https://www.hardkernel.com/shop/odroid-xu4-special-price/) / [Orange Pi 3 LTS 2GB](https://www.aliexpress.us/item/3256804169070057.html) ($45)  

1080p local/streaming content + Web Browsing (standard), Windows: Used: >= [SFF/USFF PC - CPU >= i5-7500T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=\(hp%2Cdell%2Clenovo\)+\(i5-7500%2Ci5-8400\)+\(sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini\)+ssd&_sacat=179&LH_BIN=1&LH_TitleDesc=0&_sop=15&_udhi=175&LH_ItemCondition=2010%7C2020%7C3000) ($75) OR New: >= [N95/N100 Mini PC](https://www.amazon.com/Beelink-Desktop-Computer-Ethernet-Family-NAS/dp/B0BWDGVCV7) ($150)   

4K local/streaming content + Web Browsing (standard), Windows: Used: Intel i3 8th Gen [NUC (NUC8I3BEH)](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=nuc+%288i3%2C8i5%2C8109u%2C8130u%2C8th%29&_sacat=179&LH_TitleDesc=1&_odkw=nuc+%288i3%2C8i5%2C8109u%2C8130u%29&_osacat=179&_sop=15&LH_PrefLoc=2) ($150) OR New: [Beelink SEI 11](https://www.amazon.com/s?k=beelink+sei11&i=electronics&crid=2WL5SNSMMT01O&sprefix=beelink+sei11%2Celectronics%2C141&ref=nb_sb_noss_2) ($300)  

Media Server (no/1080p transcoding): Used: [SFF/USFF PC - CPU >= i3-7100T, 4GB RAM, SSD](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%28hp%2Cdell%2Clenovo%29+%28i3-7100%29+%28usff%2Cusdt%2Csff%2Cdt%2Ctiny%2Cmicro%2Cmini%29+ssd&_sacat=179&LH_TitleDesc=0&_fsrp=1&_odkw=%28hp%2Cdell%2Clenovo%29+%28i3-7100t%2Ci3-7100%29+%28usff%2Cusdt%2Csff%2Cdt%2Ctiny%2Cmicro%2Cmini%29+ssd&_osacat=179&LH_BIN=1&_sop=15&_udhi=150) ($60) OR New: >= [N95/N100 Mini PC](https://www.amazon.com/Beelink-Desktop-Computer-Ethernet-Family-NAS/dp/B0BWDGVCV7) ($150)  

Media Server (4k transcoding):  Used: [SFF/USFF PC - CPU >= i5-7500T, 8GB RAM, SSD](https://www.ebay.com/sch/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=\(hp%2Cdell%2Clenovo\)+\(i5-7500%2Ci5-8400\)+\(sff%2Cdt%2Cmt%2Cusff%2Cmicro%2Ctiny%2Cmini\)+ssd&_sacat=179&LH_BIN=1&LH_TitleDesc=0&_sop=15&_udhi=175&LH_ItemCondition=2010%7C2020%7C3000) ($75) OR New: >= [N95/N100 Mini PC](https://www.amazon.com/Beelink-Desktop-Computer-Ethernet-Family-NAS/dp/B0BWDGVCV7) ($150)   

Network Storage: [Storage Setup Guide](/htpc-wiki/storage)

Everything else: [Sample Builds/Pre-builts](/htpc-wiki/sample-builds)  

*HD Audio means Dolby TrueHD, DTS-HD, DTS:X, and/or Lossless version of Dolby Atmos*

<!-- Section -->

## Asking for help

If you can't find an answer to your question in this FAQ, and are planning to post on the subreddit for help, please give as much information as possible.  

We ask that you answer the following questions and paste them in your post, otherwise your post may be removed for lack of details.  

Do NOT ask for help with playing media on [laptop screens or PC monitors](/htpc-wiki/faq#displays).

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

## What hardware should I choose for my HTPC?

Use a tool like [PCPartPicker](http://www.pcpartpicker.com) to see prices for hardware across several vendors and optionally to make sure pieces of a build fit together before you buy.  
Don't discount the secondary and used markets for hardware, especially when prices are high due to demand and/or scarcity. Ebay and aliexpress are good places to start.  

<!-- Sub-Section -->

### Cases

Cases come in varying shapes and sizes, with numerous features, and at varying price levels. You can spend $30 on a case. You can spend $200. Cases tend to be very personal and subjective, so we'll recommend a bunch in specific types and you can choose.  

First, choose a case that fits the space you will put it in. For HTPCs, there are cases that are meant to fit inside media cabinets (where space and dimensions are a concern), 
looking like just another piece of equipment, short and wide. If this is a frontend player in such a space, media watching is usually not the place you want to be distracted by RGB, so choose a case that blends in, rather than stands out. Smaller cases also tend to be hotter and therefore louder, due to smaller fans and heatsinks. Be mindful of this.  

Second, choose a case that will fit your motherboard and the components in it, paying special attention to the motherboard/cpu cooler/psu.  
It should be as large as the motherboard. For instance, don't use a Mini-ITX case with a Micro-ATX motherboard ([Micro-ATX > Mini-ITX](/htpc-wiki/reference)). But you may be able to use a Micro-ATX case with a Mini-ITX motherboard.  
Be aware of the PSU size. Some cases may take a regular ATX sized PSU, while others may take only SFX, TFX or even Pico sized PSUs. **Avoid** cases where you need a Flex ATX PSU as the fans are small and loud.  

**If you don't have specific requirements and/or just want something decent to build around without much thought, look at the [Silverstone ML03/ML04](https://www.amazon.com/SilverStone-Technology-Aluminum-Micro-ATX-ML03B/dp/B004GGUAUE/) and the [sample builds](/htpc-wiki/sample-builds) wiki page.**  

Here are some popular case options by size:  

SIZE/SHAPE|BRANDS
:--|:--
Tiny (Pico/Flex PSUs, no dGPU)|Inwin **[Chopin](https://www.amazon.com/InWin-Chopin-Mini-ITX-stickers-Aluminum/dp/B01N091225/)/[BQ656T](https://www.amazon.com/WIN-150W-Mini-ITX-Black-BQ656T-AD150TB3/dp/B01LVV6WVU)**, **[ASRock Deskmini](https://www.asrock.com/nettop/AMD/DeskMini%20X300%20Series/index.asp)**, [Rgeek L65/L80S/C01](https://www.amazon.com/RGEEK-Cover-Holes-Aluminum-Computer/dp/B07Q7NGLW6), Realan H60/H65S/H80, [Goodisory A01](https://www.amazon.com/Goodisory-Aluminum-Mini-ITX-Desktop-Computer/dp/B07GYP2TWC), [MITXPC MX500](https://www.amazon.com/MITXPC-MX500-USB3-Compact-Mini-ITX-Fanless/dp/B0728DX73X), [Geeek A1/A30](https://www.geeekstore.com/product-category/case/)
Cube|*ITX:* ASRock Deskmeet, Raijintek Metis, Silverstone SG13/SG05, Golden Field N-1, Thermaltake Core V1 *uATX:* [Jonsbo C6](https://www.newegg.com/p/2AM-006A-000C4?item=9SIAY3SJTA9704) 
Long Cube|*ITX:* Sharkoon QB One, Fractal Design Core 500, **[Node 304](https://www.fractal-design.com/products/cases/node/node-304/black/)**, Coolermaster Elite 130, *uATX:* Silverstone SG02/SG11
Short - media cabinet|*ITX/uATX/ATX:* [**Silverstone ML**/RVZ/GD](https://www.silverstonetek.com/en/product/computer-chassis/?filter=HTPC_Desktop,grandia,milo,RAVEN&sort=Newsest) series. *ITX:* [Node 202](https://www.fractal-design.com/products/cases/node/node-202/black/), [Fractal Ridge](https://www.fractal-design.com/products/cases/ridge), Raijintek Pan, Inwin [BP](https://www.in-win.com/en/computer-chassis/bp-series)/[BQ](https://www.in-win.com/en/computer-chassis/bq-series). *uATX:* Apex DM-387/MI-008, Inwin BL/CE (BL040/CE685), Antec VSK2000.
Fanless|[HDPLEX](http://www.hdplex.com), [Streacom](http://www.streacom.com/products/), [Akasa Maxwell Pro, Euler M/S/T](https://www.akasa.com.tw/update.php?tpl=product/product.list.tpl&type=Fanless%20Chassis&type_sub=Fanless%20Mini%20ITX)
NAS|[Wiki: DIY NAS Case List](/htpc-wiki/storage#diy-nas-case-list), Fractal **[Node 804](https://www.fractal-design.com/products/cases/node/node-804/Black/)**/Node 304/Define R5, Jonsbo N1/N2/N3, Silverstone CS380/DS380/GD07/GD08, iStarUSA S-35
Full dGPU (Sandwich)|**[Geeek G1/M5/A40/A50/A60](https://www.geeekstore.com/product-category/case/)**, Raijintek Ophion ALS, Nouvolo Steck, Lian Li A4, Fractal Terra, Sliger SM550, SGPC K49
Full dGPU (Other)|[Silverstone GD (short), RVZ/ML07/ML08 (shorter), SG13 (cube)](https://www.silverstonetek.com/en/product/computer-chassis/?filter=Small_Form_Factor,HTPC_Desktop,grandia,RAVEN,sugo&sort=Newsest), [Jonsbo C6](https://www.newegg.com/p/2AM-006A-000C4)/C2, Node 202/304, Core 500 
ATX mobo|**[Silverstone GD09 - 27L/$95](https://www.silverstonetek.com/en/product/info/computer-chassis/GD09/)**, [GD11 - 31L/$170](https://www.silverstonetek.com/en/product/info/computer-chassis/GD11/), [SSUPD Meshroom S - 15L/$160](https://www.ssupd.co/products/new-meshroom-s), [SFFTime P-ATX - 10L/$170](https://www.sfftime.com/p-atx), Sliger Cerberus X - 24L/$265, [HDPLEX H5 - 17L/$300](http://www.hdplex.com/hdplex-h5-fanless-computer-case.html), Thermaltake Core G3 - 23.6L/EoL
uATX & small|Realan 2007C E-Mini, CEMO M1, Inwin [CJ](https://www.in-win.com/en/computer-chassis/cj-series/APAC)/[CK](https://www.in-win.com/en/computer-chassis/ck-series/APAC) (CK709), [Inwin BK](https://www.in-win.com/en/computer-chassis/bk-series/APAC) (BK623) (dGPU), [Jonsbo C6](https://www.newegg.com/p/2AM-006A-000C4?item=9SIAY3SJTA9704) (dGPU)
SFF Tower|*ITX:* **[CoolerMaster NR200](https://www.coolermaster.com/catalog/cases/mini-itx/masterbox-nr200/)**, [Geeek M5](https://www.geeekstore.com/product-category/case/), Cougar QBX, [CoolerMaster H100](https://www.coolermaster.com/catalog/legacy-products/cases/mastercase-h100/), [SSUPD Meshlicious](https://www.ssupd.co/products/meshlicious) *uATX:* [Sama IM01](https://pcpartpicker.com/product/pfvdnQ/sama-im01-microatx-mini-tower-case-im01), Jonsbo [U3](https://www.jonsbo.com/en/products/u3black.html) / [V4](https://www.jonsbo.com/en/products/v4black.html)
Water Cooling|Silverstone GD11, [SFFTime N-ATX](https://www.sfftime.com/n-atx), SSUPD Meshroom S, CoolerMaster NR200, Lian Li A4-H2O

<!-- Sub-Section -->

### CPUs

The CPU you choose for a HTPC will be heavily influenced by what your usage profile for the system looks like. 
You could be using it as a frontend player, a dual-duty gaming pc or a backend media server, so there isn't necessarily a one size fits all to the CPU you should choose. 

The GPU (whether it's integrated into the CPU or a separate, discrete GPU) tends to be a more important piece of the puzzle. All CPUs in this section will have iGPUs built into them. If you want a dGPU, we'll talk more about that in the Graphics section below. For CPU characteristics in general, we'll give broad recommendations here.

1. You should generally have a CPU that generates the least amount of heat (TDP) that you'll need. Faster and more powerful is not always better. The more powerful your 
CPU, the higher the TDP will be, the more heat will be generated, the louder your fans will be. If the HTPC will be in your listening environment, the last thing you want to 
hear is a loud fan. So stick with CPUs with TDPs <= 65W. CPU temps <= 80C under load are fine; anything higher than that is generally frowned upon for CPU longevity, esp 90+. Use Open Hardware Monitor/HwInfo64 to monitor your temps.  
2. You shouldn't need anything more than a 4 core CPU for a frontend player. A backend server may require 6 core if doing something intensive like handbrake transcoding. 
3. Don't forget a CPU cooler for your CPU, IF one is not already included. Ryzen APUs and non-K Intel CPUs DO come with a stock cooler, but you can do better if funds and space allow it. 
We have a whole section on cooling below. Remember: bigger, slower fans are better than smaller, faster fans.  

Below are the minimum CPUs required for each scenario and a recommendation. **All have integrated graphics and a dGPU is not required**. The recommendations may change depending on your budget, regional availability, space/power requirements, and whether you want new or second-hand parts. If you're not sure, post and ask us for a rec based on your detailed use-case.  

- **Best All-Rounder: AMD Ryzen 4600G, Intel i3-12100**  

- 1080p, No gaming: Intel >= i3/i5/i7-7xxx iGPU, Pentium G4xxx or Apollo/Gemini Lake J3xxx, AMD Athlon 3000G, AMD >= Ryzen 3 2200G APU (REC: Intel G7400)  

- Emulators: 1080p: AMD >= Ryzen 5 3400G APU. 720p: AMD >= Ryzen 3 3200G APU (REC: Ryzen 4600G)  

- Light gaming: AMD >= Ryzen 3 3200G APU (REC: Ryzen 5600G)  

- Medium gaming: AMD >= Ryzen 5 3400G APU (REC: Ryzen 5700G)  

- 4K HDR: Intel >= i3/i5/i7-7xxx iGPU, AMD Athlon 3000G, AMD >= Ryzen 3 2200G APU (REC: Ryzen 4600G)  

- 4K Netflix: >= Ryzen 3 3200G iGPU, Intel >= i3/i5/i7-7xxx iGPU  (REC: Ryzen 4600G)  

- AV1 decoding: >= Intel i3/i5/i7-11xxx iGPU, >= Ryzen 7xxx/6600U iGPU (REC: Intel i3-12100)  

- UHD Blu-Ray disc playing: Intel i3/5/7/9 7th-10th Gen iGPU ONLY + [Motherboard BIOS supporting Intel SGX](/htpc-wiki/hdmi20) (REC: Intel i3-10100)  

- HDMI 2.1 4K@120Hz: >= Ryzen 7xxx/6600U iGPU  

- Plex Transcoding: Intel >= i3/i5/i7-7xxx iGPU (REC: Intel i3-12100)  

<!-- Sub-Section -->

### GPUs/Graphics

**In most cases, a CPU that has an integrated GPU as recommended above will work fine for new HTPCs**. If you need more than what they provide or you're adding onto an existing system, then a dGPU is warranted. Since HTPCs are in listening environments and tend to be small, low TDP, low profile dGPUs are what we aim for to keep heat and noise in check, wherever possible. You can pair these up with CPU without the integrated GPUs. For Intel these are 'F' tagged skus. For AMD, non 'G' tagged skus.  

Some features like HDR, 4K and protected content will restrict you to certain models. For instance, for 4K netflix you cannot use a Nvidia GT 1030 or GTX 1050 with only 2GB of VRAM. You need at least 3GB, so do not ignore the ">=" below in the 4k Netflix recommendations. See the 4K/HDR sections for more system requirements.  

Below are the minimum requirements for each scenario and a recommendation. The recommendations are generalized and may change depending on your budget, regional availability, space/power requirements, and whether you want new or second-hand parts. If you're not sure, post and ask us for a rec based on your detailed use-case.  

- **Best All-Rounder: AMD RX 6400**  

- 1080p H264, 4k@30Hz video out: AMD Radeon R5 240/HD 8570 (REC: Dell R5 240)  

- 4K Local HDR+4K Youtube HDR: Nvidia >= GT 1030 GDDR5, AMD >= 5x00/6x00 (REC: Used: GTX 1050 Ti, New: RX 6400)  

- 4K Netflix: Nvidia >= GTX 1050 3GB, AMD >= RX 550/5x00/6x00 (REC: Used: GTX 1050 Ti, New: RX 6400)  

- 4K Netflix+Youtube+Local HDR: Nvidia >= GTX 1050 3GB, AMD >= RX 6x00 (REC: Used: GTX 1050 Ti, New: RX 6400)  

- AV1 decoding: >= Intel Arc A3xx/Nvidia RTX 3050/A2000/AMD RX 6600 (REC: Intel Arc A380)  

- Emulation: Nvidia >= GT 1030 GDDR5, AMD >= 5xx/5x00/6x00 (REC: Used: GTX 1050 Ti, New: RX 6400)  

- HDMI 2.1 4K@120Hz: >= Nvidia RTX 3050/AMD RX 6400 (REC: RX 6400)  

- UHD Blu-Ray disc playing: Not supported. Intel iGPU only.

- Plex Transcoding: [Elpamsoft GPU transcode tables](https://www.elpamsoft.com/?p=Plex-Hardware-Transcoding) (REC: Quadro P600/GTX 1050 Ti)  

- Best low-profile card (4K Netflix+Youtube+Local HDR): AMD RX 6400 / Nvidia GTX 1650 (REC: Used: GTX 1050 Ti, New: RX 6400)  

- madVR upscaling/tonemapping: >= GTX 1060 6GB / AMD RX 5600 (Rec: GTX 1660)  

**GPU/CPU Feature Set Matrix:**

CPU/GPU										|	HEVC 8b	|HEVC 10b	|AV1	|4K NETFLIX	|HDMI		|DP		|VP9 8b	|VP9 10b	|HDR		|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
Intel i3-i7 2xxx-3xxx (DT)					|	N		|	N		|	N	|	N		|1.4		|1.2	|	N	|	N		|	N		|Sandy/Ivy Bridge
Intel i3-i7 4xxx-6xxx (DT)					|	Y		|	N		|	N	|	N		|1.4		|1.2	|	N	|	N		|	N		|Haswell/Broadwell/Skylake
Intel i3-i9 7xxx-10xxx (DT)					|	Y		|	Y		|	N	|	Y (2)	|1.4 (1)	|1.2	|	Y	|	Y		|	Y (2)	|Kaby/Coffee/Comet Lake
Intel i3-i9 11xxx-14xxx	(DT)				|	Y		|	Y		|	Y	|	Y		|2.1 (7)		|1.4 (12)	|	Y	|	Y		|	Y		|Rocket/Alder/Raptor Lake
Intel G39/45/46/49/54/55xx (DT)				|	Y		|	Y		|	N	|	Y (2)	|1.4 (1)	|1.2	|	Y	|	Y		|	Y (3)	|Kaby/Coffee/Comet Lake
Intel G69xx/G74xx (DT)				|	Y		|	Y		|	Y	|	Y		|2.1 (7)		|1.4	|	Y	|	Y		|	Y		|Alder Lake
Intel z3xxx/z8xxx/J30xx/J31xx/J37xx/N30xx (EM)	|	Y		|	N		|	N	|	N		|1.4		|1.2	|	N	|	N		|	N		|Braswell/Cherry Trail
Intel J33xx/J34xx/N33xx/N34xx/N4200 (EM)			|	Y		|	Y		|	N	|	Y (2)	|1.4 (1)	|1.2	|	Y	|	N		|	Y (3)	|Apollo Lake/Goldmont
Intel J4xxx/J5xxx/N40xx/N41xx/N50xx (EM)			|	Y		|	Y		|	N	|	Y		|2.0		|1.2	|	Y	|	Y		|	Y (3)	|Gemini Lake/Goldmont+
Intel N45xx/N51xx/N55xx/N6xxx (EM)				|	Y		|	Y		|	N	|	Y		|2.0		|1.2	|	Y	|	Y		|	Y	|Jasper Lake/Tremont
Intel 10xxG/10xxxU/10xxxH (EM)					|	Y		|	Y		|	N	|	Y		|2.0		|1.2	|	Y	|	Y		|	Y		|Ice Lake
Intel 11xxG/11xxxU/11xxxH (EM)					|	Y		|	Y		|	Y	|	Y		|2.1 (7)		|1.4	|	Y	|	Y		|	Y		|Tiger Lake
Intel 12xx(U/P/H)/13xx(U/P/H)/Nxxx (EM)					|	Y		|	Y		|	Y	|	Y		|2.1 (7)		|1.4	|	Y	|	Y		|	Y		|Alder/Raptor Lake
Intel 14xx(U/P/H) (EM)					|	Y		|	Y		|	Y	|	Y		|2.1		|2.1	|	Y	|	Y		|	Y		|Meteor Lake
Intel ARC Axxx					|	Y		|	Y		|	Y	|	Y		|2.0 (8)		|2.0	|	Y	|	Y		|	Y		|Alchemist
AMD Ryzen 2xxxG-3xxxG/2x0G-3x0G (DT)			|	Y		|	Y		|	N	|	Y (4)	|2.0		|1.2	|	Y	|	Y		|	Y		|Raven Ridge/Picasso & Vega
AMD Ryzen 4xxxG-5xxxG (DT)			|	Y		|	Y		|	N	|	Y	|2.0		|1.4	|	Y	|	Y		|	Y		|Renoir/Cezanne & Vega
AMD Ryzen 2xxxU-3xxxU (EM)							|	Y		|	Y		|	N	|	Y (4)	|2.0		|1.2	|	Y	|	Y		|	Y		|Raven Ridge/Picasso & Vega
AMD Ryzen 4xxxU-5xxxU (EM)							|	Y		|	Y		|	N	|	Y	|2.0		|1.4	|	Y	|	Y		|	Y		|Renoir/Cezanne & Vega
AMD Ryzen 6xxxU (EM)									|	Y		|	Y		|	Y	|	Y		|2.1		|2.0	|	Y	|	Y		|	Y		|Rembrandt & RDNA2
AMD Ryzen 7xxx (DT)									|	Y		|	Y		|	Y	|	Y		|2.1 (11)		|2.0	|	Y	|	Y		|	Y		|Raphael & RDNA2
AMD RX 4xx/5xx								|	Y		|	Y		|	N	|	Y		|2.0		|1.4	|	N	|	N		|	Y		|Polaris
AMD RX Vega 56/64/VII						|	Y		|	Y		|	N	|	N		|2.0		|1.4	|	N	|	N		|	Y		|RX Vega
AMD RX 5xxx									|	Y		|	Y		|	N	|	Y		|2.0		|1.4	|	Y	|	Y		|	Y		|Navi/RDNA
AMD RX 6xxx									|	Y		|	Y		|	Y (6)	|	Y		|2.1		|1.4	|	Y	|	Y		|	Y		|Navi/RDNA2
AMD RX 7xxx									|	Y		|	Y		|	Y	|	Y		|2.1		|2.1	|	Y	|	Y		|	Y		|Navi/RDNA3
Nvidia GTX/RTX 10/16/20						|	Y		|	Y		|	N	|	Y (5)	|2.0		|1.4	|	Y	|	Y (9)		|	Y		|Pascal/Turing
Nvidia RTX 30xx								|	Y		|	Y		|	Y	|	Y		|2.1		|1.4	|	Y	|	Y		|	Y		|Ampere
Nvidia RTX 40xx								|	Y		|	Y		|	Y	|	Y		|2.1		|1.4	|	Y	|	Y		|	Y		|Ada Lovelace

*Footnotes*  
(DT) Desktop  
(EM) Embedded. Mobile, Mini PC, etc..  
(HEVC 8b/VP9 8b) Used for HW accel 4k non-HDR  
(HEVC 10b/VP9 10b) Used for HW accel 4k HDR  
(1) [HDMI 2.0 possible w/specific mobo](/htpc-wiki/hdmi20)  
(2) [Only with Windows and HDMI 2.0 mobo/vendor-specific DP adapter](/htpc-wiki/hdmi20)  
(3) Only with libreelec OS and specific SKUs  
(4) Requires >= 3300U or >= 3200G  
(5) Requires >= 1050 3GB/1050 Ti  
(6) Requires >= RX 6600  
(7) Only provides HDMI 2.0 bandwidth/resolutions  
(8) HDMI 2.1 available on specific SKUs w/PCON from DP  
(9) [Not GTX 1060/1070/1080](https://en.wikipedia.org/wiki/Nvidia_NVDEC)  
(11) 4k@120 Hz 4:2:2 10-bit HDR - 32 Gbps (mobo limited)  
(12) DP 2.1 - 40 Gbps with usb available on specific 13xxx mobo SKUs  

<!-- Sub-Section -->

### Motherboards

Motherboards are sometimes a matter of preference, however many of the higher-end features, like integrated RAID support, RGB, and multiple network interfaces, aren't particularly helpful in a HTPC environment.  
The best values are in motherboards with the Bxxx chipsets for Intel/AMD, so that's what we recommend.  
Even cheaper are the bargain basement chipsets like Intel [Hx10 (Intel)](https://en.wikipedia.org/wiki/List_of_Intel_chipsets#600/700_Series_chipsets) e.g. H510/H610. and AMD [Ax20 (AMD)](https://en.wikipedia.org/wiki/List_of_AMD_chipsets#AM4_chipsets) e.g. A320/A520; they are also fine for a basic build, they just skimp on features a little more, like no PCIe 4, limited/no memory overclocking and/or limited SATA ports.  
For form factor, Mini-ITX boards are usually preferred for their smaller size where space is at a premium (though they are more expensive), followed by Micro-ATX which are a little bigger in size (and which tend to be the least expensive, so are the best value). Full ATX sized boards are large and aren't particularly useful here.  
Make sure you check the mfgr specs/support page for any potential motherboard you want for your CPU, as the chipset in combination with the BIOS version may dictate what CPUs are supported.  
Shoot for spending $100-$200 for a motherboard, with $125 being a good starting point.  

Example Combinations:  
- AMD: Ryzen 4600G + B550: [MicroATX](https://pcpartpicker.com/list/mcFhFg), [Mini-ITX](https://pcpartpicker.com/list/NWTfd9)  
- Intel: Core i3-12100 + B660: [MicroATX](https://pcpartpicker.com/list/fDQNgb), [Mini-ITX](https://pcpartpicker.com/list/mFXf9r)  

BRANDS/MODELS:  
Asus, MSI, Gigabyte, ASRock. Avoid Biostar!  

<!-- Sub-Section -->

### Displays

See [/r/4kTV](https://www.reddit.com/r/4kTV), [/r/Televisions](https://www.reddit.com/r/Televisions) and [/r/Projectors](https://www.reddit.com/r/Projectors) sub-reddits.  

We will not support Laptop Screens or PC Monitors as Home Theater display devices due to: lack of low (23p-25p) refresh rate matching support, lack of ARC/eARC, poor contrast ratios (< 3000:1), upscaling and HDR capabilities compared to TVs, along with non-standard (1440p) resolutions that can't be passed-through sound systems.  

<!-- Sub-Section -->

### Memory/RAM

Most HTPC applications do not need very much RAM. You can get away with 4GB of RAM, especially on Linux-based OSes. On Windows, shoot for at least 8GB nowadays, unless you're on a strict budget.  

If you're playing 4K media or doing some gaming with an CPU-integrated GPU/APU, you will get a lot better performance if you use 2 memory modules instead of 1 (e.g. 2x4GB for 8GB total or 2x8GB for 16GB) in a dual-channel configuration, with >= 3200 Mhz frequency and XMP enabled in your BIOS.  

BRANDS/MODELS:  
*- Quality:* Corsair, G.Skill, Crucial (REC: 2x8GB DDR4-3600 Corsair Vengeance LPX)  
*- Budget:* Patriot, Teamgroup, Silicon Power (REC: 2x8GB DDR4-3200 Silicon Power Gaming)  
*- Low Profile:* G.Skill Aegis/Patriot Signature/Crucial Green (31.25mm), Teamgroup Elite (31.5mm), Teamgroup Vulcan Z (31.6mm), Corsair Vengeance LPX (34mm), HyperX Fury (34.1mm)  

[Example PCPartPicker RAM search](https://pcpartpicker.com/products/memory/#xcx=0&U=4&t=14&S=3200,6600&Z=8192002,16384002,32768002&sort=price&page=1&R=5,4,3)  

<!-- Sub-Section -->

### Storage/HDDs/SSDs

Your OS should be stored on a SSD. Shoot for at least a 2.5" 250GB SATA drive. A SATA SSD will be 30-50x faster than a HDD at OS operations. A M.2 NVMe SSD with transfer rates of 1500 MB/s will be around 2x faster than a SATA SSD and is the best option, while reducing cable clutter in the process. A high-end M.2 NVMe SSD @ 3000 MB/s will be 5x faster than a SATA SSD, but does not make sense price-wise unless you have highly sequential read/write tasks (which shouldn't happen on an OS drive).  

Your media content should be stored on HDDs. Internal drives for media are preferred, but external drives are also fine. 2.5" HDDs are ok for the smallest cases, but capacities are limited to 5 TB, so if you need larger, you'll have to go to 3.5". If using external drives, make sure power management features in your OS don't disconnect a USB drive after a certain period of time. 
You can also buy external drives and "shuck" the drives out of them to use internally in your HTPC, which tends to be cheaper. Check the [Storage wiki page](/htpc-wiki/storage) page for prices/recs of internal/external drives.  

There are a very few cases where a SSD should be used for media or non-OS data: 

1. If absolute silence is required, such as in a bedroom where the HTPC will remain on 24/7.
2. If you're running Plex Media Server, an SSD should be used for its metadata directories (for quick access during media browsing) and also for temporary media transcoding storage.
3. If you're playing large games. Game loading does benefit from having a SSD. A SATA one is fine.

BRANDS/MODELS:  
SSDs:  
*- Quality:* Samsung, WD Black, SK Hynix, Sabrent, Crucial (OS Drive REC: Samsung 970 Evo Plus)  
*- Budget:* Teamgroup, Silicon Power, Inland, Kingston, WD Blue (OS Drive REC: Teamgroup MP33).  
HDDS: Ultrastar, Seagate Exos, WD Red  
[Example PCPartPicker SSD search](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=128000000000,20000000000000&t=0&f=3,122080&sort=price&R=5,4,3)  

<!-- Sub-Section -->

### Optical Drives

NOTE: UHD/4k blu-ray **disc** playback is not recommended due to hardware restrictions. See [here](https://www.cyberlink.com/support/faq-content.do?id=19144) and [here](/htpc-wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility)   

If you can meet the restrictions, then buy an Official Playback drive and use PowerDVD.  

If you **can't** meet the restrictions, then either (in order of preference):  

 1. Buy a MakeMKV-supported drive and Rip the discs to digital with makemkv

 2. Buy a [standalone player](https://www.google.com/search?q=panasonic+ub420+ub820&oq=panasonic+ub420+ub820) for your HT system.  

 3. Buy a UHD Friendly drive and Play the discs using Redfox AnyDVD HD and your favorite media player

*DVD/Blu-Ray:*  
Internal: LG WH14NS40/ASUS BW-16D1HT, Pioneer, Asus  
External, Slim: Archgon MD-3102S/LG BP60NB10/BP50NB40 (External, Slim)  

*UHD Blu-Ray (for ripping or AnyDVD playback):*  
See [MakeMKV forum post on recommended drives/FW](https://forum.makemkv.com/forum/viewtopic.php?f=16&t=19634)  

*UHD Blu-Ray (for Official Playback/ripping):*  
Internal: LG WH16NS60  
Internal, Slim: LG BU40N  
External, Slim: Archgon MD-8107S/Buffalo BRUHD-PU3/LG BP60NB10  

<!-- Sub-Section -->

### Power Supplies/Power Usage

**Power Supplies**

Being that a HTPC tends to run 24/7/365, builders are always trying to get the best bang for their buck when it comes to performance/power. Choosing the proper power supply is a balance between power, price, reliability and sometimes even noise.  

TYPES:  

1. [ATX](https://pcpartpicker.com/products/power-supply/#xcx=0&t=2&sort=price&page=1): Very common; large, high compatibility, well-priced. Used for medium to large cases.
2. [SFX](https://pcpartpicker.com/products/power-supply/#xcx=0&sort=price&t=10): Smaller in size than ATX, but expensive. Used for small cases.
3. [TFX/Flex](https://pcpartpicker.com/products/power-supply/#xcx=0&sort=price&t=13,6,8,10): Long and skinny. Smaller fans and lower power output than ATX/SFX. Used for small cases and few attached devices where noise isn't an issue, because these are the loudest PSUs.
4. [Pico](https://www.mini-box.com/s.nl/sc.8/category.13/.f): Super small. No fan, low power output, bulk of PSU is the AC adapter which is outside the case. Used for a <= 65W CPU and 1-2 drives. Excellent for tiny cases where space is at a premium and not many peripherals will be used.

MODULARITY:  

Semi-modular ATX/SFX PSUs strike the best balance between price and cable space used. We would recommend this modularity at the minimum.

1. Non-modular: All possible power wires are connected to the PSU
2. Semi-modular: Best balance between cable space and price. 24-pin motherboard and 4/8-pin cpu eps cables are connected to the PSU. All other cable connections are optional.
3. Fully-modular: All cable connections are optional. 

SIZING:  

Don't be tempted to go with the "bigger is better" philosophy. If you've designed your HTPC build well for your needs, you shouldn't need a huge power supply.

First, you should find out how much power you'll be using. Use the power calculator [here](https://outervision.com/power-supply-calculator) for that.

Next, what kind of PSU should you get? Well, the power calculator will offer a recommended one, but there are many choices.

PSUs are rated by wattage and efficiency. For efficiency there's an 80+ rating system with ratings like 80+, 80+ Bronze, Silver, Gold, etc..

A higher efficiency means a lower power bill, but this comes with a higher PSU cost. So it's a balancing act. If you're saving $10 a year in power because you're using a Gold PSU versus a Bronze PSU, but the Gold PSU costs $60 more, well, you're not breaking even until year 6.

Efficiency is also tied to how much load you put on the PSU. A PSU is the most efficient when it's at 50% of its maximum load. So if you expect to be using 150W consistently, then a 300W PSU will be ideal. 

For most HTPC builds (but check the calculator!), we usually recommend a 80+ Bronze PSU in the 300-400W range. Problem is, these days, most PC builds are around gaming and PSU sizes 
tend to trend higher, so finding a good selection of lower wattage PSUs isn't easy. You may have to go up to a 500W PSU. Sometimes you will find a case with a lower wattage 
(200W-250W) PSU built right-in.  

BRANDS/MODELS:  
ATX: Seasonic (Focus/S12/GM), Super Flower (Leadex), EVGA (GA/G5/GD), Corsair (RM/CXM), Silverstone (ST/SX). Shoot for a warranty of 5-10 years.  
[Example ATX/SFX PSU search](https://pcpartpicker.com/products/power-supply/#m=8,337,169,50,11,14,106,229,71,63,441,56&sort=price&A=200000000000,1000000000000&e=6,5,4,3,2,1)  
Silent (< 20 dBA): [Phanteks Amp](https://www.cybenetics.com/index.php?option=database&cert=1&bdg=4&volts=1&manfID=83), [Super Flower Leadex III Gold](https://www.cybenetics.com/index.php?option=database&params=1,0,55), [be Quiet! Straight Power 11](https://www.cybenetics.com/index.php?option=database&params=1,0,22), [Corsair RM550x](https://www.cybenetics.com/index.php?option=database&params=1,0,28)  
SFX: Seasonic Focus SGX, Silverstone ST30SF/SX, Corsair SF, EVGA GM, FSP Dagger Pro Gold  
Pico: [HDPlex](https://hdplex.com/hdplex-fanless-250w-gan-aio-atx-psu.html), [Mini-Box](https://mini-box.com), [RGeek](https://www.amazon.com/stores/RGEEK/page/616B17E4-8578-4D17-B851-98993644408F?ref_=ast_bln)  
Flex: [Enhance](https://www.geeekstore.com/product-category/power-supply/), [Silverstone](https://www.silverstonetek.com/en/product/power-supplies/?page=1&filter=TFX_Flex_ATX&sort=Newsest): mod w/Noctua 40mm fan for low noise.  

**Power Usage**

Now that you know what kind of PSU you should look for, how much will the power cost? Well, we're going to assume 24/7/365 operation here.

General rule of thumb is that your monthly power cost will be about 8.5% of the wattage. So, if you're using 100W, your monthly power cost will be $8.5 (100*.085).

If you want to get the ACTUAL cost, using the avg KwH cost in the U.S. of about $.12, we use:

**Wattage * Hours used / 1000 * KwH cost = Power Cost in $**

So let's take our 100W example for 24/7 usage in a month of 732 hours (24 hrs*30.5 days).

(100 * 732) / 1000 * .12 = $8.78/month

<!-- Sub-Section -->

### Cooling

In almost all circumstances, the manufacturer-supplied CPU heat sink and fan is sufficiently cool, and it's not useful to immediately jump to an expensive aftermarket cooler until you know you need one. 

We recommend that you assemble the system without supplemental cooling, then add an additional/replacement case fan or cpu cooler only if you find that the temperature or noise is too high.  
In that case, a larger, slower fan is quieter than a smaller, faster fan. 

Avoid putting the case in a space with no airflow (e.g. enclosed entertainment centers). This will just heat the components no matter how many fans you throw at it, especially if you're 
using a high TDP/Watt CPU. If you need, cut holes in the back of the enclosed space at the minimum or, ideally, add a fan to that back space to expel the hot air from inside.  Look at [AC Infinity](https://acinfinity.com/quiet-cabinet-fans/) fans/grills which can be found in [USB](https://acinfinity.com/quiet-usb-fans/) and [AC power](https://acinfinity.com/ac-axial-fans/) options, to mount outside of your PC.  

As stated in the CPU section, if your CPU is <= 80C temp-wise, you're ok. SSD <= 60C is ok. HDD <= 40C is ok.  

Make sure that when you are researching builds, if you are looking at a low-profile case, that you take its height into account. Some will not allow for the height of the stock CPU cooler.  

BRANDS/MODELS:  
Noctua, Thermalright, be Quiet!, Arctic, Scythe  

For case fans, look at the Arctic P12 series for affordability or the Noctua A series for the best.  
For cpu coolers, look at the Noctua [NH-L9i](http://noctua.at/en/products/cpu-cooler-retail/nh-l9i)/[NH-L9a](http://noctua.at/en/products/cpu-cooler-retail/nh-l9a)/L9x65/L12S, Thermalright AXP Series, Scythe Big Shuriken and the Arctic Freezer [11 LP](https://www.arctic.ac/us_en/freezer-11-lp.html) for small cases and the Noctua NH-D12L, ID Cooling SE-224-XT, Thermalright Peerless Assassin or Arctic Liquid Freezer II AIOs for large cases.  

Check our [CPU Coolers](/htpc-wiki/cpucoolers) wiki page for an extended list.  

<!-- Sub-Section -->

### Surge Suppression

Surge suppressors are a good idea for protecting your equipment, especially in regions where lightning is or voltage spikes are prevalent.  

Any of the options below are fine in general, though the HT10DBS is preferred for the best balance. If you're paranoid about voltages, get the Furman, as most protectors will only clamp down above 330/400V.  

[Tripp Lite ISOBAR6DBS](https://assets.tripplite.com/product-pdfs/en/isobar6dbs.pdf) - 6 plug, 3330 Joules, 1440W, $250k protection, Tele/coax ($70)  

[Furman PST-8/PST-8D](https://furmanpower.com/product/15a-8-outlet-surge-suppressor-strip-w-smp-lift-and-evs/) - 8 plug, 4320 Joules, Tele/coax, Noise suppression, Extreme voltage clampdown >137V ($115)  

[Tripp Lite HT10DBS](https://assets.tripplite.com/product-pdfs/en/ht10dbs.pdf) - 10 plug, 3840 Joules, 1440W, $500k protection, Tele/coax/LAN ($120)  

Tripp Lite TLP1210SATG - 12 plug, 3600 Joules, 1800W, $250k protection, Tele/coax/LAN ($85)  

APC P10U2/P12U2 - 10/12 plug, 4320 Joules, 1400W, $300k protection, USB, No tele/coax ($35)  

Tripp Lite TLP1208TEL - 12 plug, 3345 Joules, 1800W, $150k protection, Tele ($50)  

Belkin Pivot-Plug 12 BP112230-08 - 12 plug, 4320 Joules, 1875W, $300k protection, Tele/coax ($45)  

<!-- Sub-Section -->

### Video Cables/Adapters

Refer to [this table](https://images.idgesg.net/images/article/2018/02/formatdataratetable-100750471-large.jpg) for the bandwidth and cable speed required for each resolution/refresh rate/chroma.

**HDMI Cables**

There are a LOT of HDMI cable companies floating around on the internet. Some good. Some bad.  

For 4K@60Hz or 1080p@120Hz, always get a "High Speed" cable that supports "18 Gbps". We HIGHLY recommended a cable that is "[Premium Certified](https://www.hdmi.org/spec/premiumcable)", which means that it has been tested by the HDMI spec organization up to the full 18 Gbps bandwidth and not the Standard speed of 10.2 Gbps. Do not settle for anything less than a wire thickness of 28 AWG up to 15 ft and 24 AWG up to 25 ft (lower AWG is thicker) for these passive type cables.  

You don't have to spend a lot for all of this, even Premium Certified. We recommend [Monoprice Premium Certified](https://www.monoprice.com/product?p_id=15427) or [Cable Matters Certified](https://www.amazon.com/Cable-Matters-Premium-Certified-Support/dp/B004D5EYG4) cables. Pick up a 6 footer for $8 and call it a day. You probably shouldn't be spending more than $1.75/foot unless it's something unique to your situation or from a quality, low-volume vendor like [Blue Jeans Cable](https://www.bluejeanscable.com) which we can also recommend for high-quality cables.  

You should not run normal High Speed cables over 25 ft. If you need to go further than that, look at "Active" or HDMI-over-fiber cables. We recommend [Ultra Active](https://www.monoprice.com/product?p_id=12735)/[Slim-run AV](https://www.monoprice.com/category/cables/hdmi-cables/hdmi-cables?menuDisStr=hdmi%20cables&v_Series_uFilter=SlimRun%20AV&TotalProducts=6), [RUIPRO Ultra-Slim](https://www.amazon.com/RUIPRO-Fiber-Cable-Support-Subsampling/dp/B01MDQ5JOC) or [Blue Jeans Series-3A](https://www.bluejeanscable.com/store/hdmi-cables/hdmi-cable.htm) cables. Runs over 100 ft for 4K are NOT recommended. Look [here](https://www.avforums.com/attachments/hdmi-cables-performance-evaluation-testing-report-1-_-50ft-15m-length-cables-v3-sml-3-pdf.1149898/) for cable testing results.  

For 4K@120Hz, always get a "Ultra High Speed" cable that supports "48 Gbps". We HIGHLY recommend a cable that is "[Ultra Certified](https://hdmi.org/spec21sub/ultrahighspeedcable)". Cables currently meeting this spec that we can recommend are Monoprice [8K Normal](https://www.monoprice.com/product?p_id=42674) or [8K Braided](https://www.monoprice.com/product?p_id=42682), [Club3D 1372](https://www.amazon.com/Club3D-CAC-1372-Ultra-Speed-Male-Male/dp/B07H5Y5N55), [Zeskit Maya/X-Tech](https://www.amazon.com/48Gbps-Compatible-Netflix-Playstation-Samsung/dp/B07S1CGQ9Z?ref_=ast_sto_dp) and [RUIPRO 8K](https://www.amazon.com/RUIPRO-Certified-Dynamic-Suitable-Samsung/dp/B08QTNNRS4).  

You should not run normal Ultra High Speed cables over 10 ft. The only normal cable you could run out further is the 16 ft [Zeskit Maya](https://www.amazon.com/48Gbps-Compatible-Netflix-Playstation-Samsung/dp/B07S1BNM7K) (it will be super stiff to keep signal integrity at that distance). If you need to go further than that, look at HDMI-over-fiber cables. We recommend [RUIPro 8K HDMI Fiber](https://www.amazon.com/RUIPRO-Dynamic-Flexible-Projector-Theatre/dp/B081SHJJ3C?ref_=ast_sto_dp&th=1&psc=1), [Phoossno 8K Fiber](https://www.amazon.com/Certified-Fiber-Optical-Cable-phoossno/dp/B09LYZQW93?th=1) or [Cable Matters Active 8K Fiber](https://www.amazon.com/dp/B092MWQGSF/)  

Please do NOT buy no-name cables. Do NOT buy Amazon Basic cables for 4K@60Hz.  

**Adapters/Adapter Cables**

If you need a passive Displayport to HDMI cable to just carry HD audio or to only do 4K@30Hz, [Amazon Basics](https://www.amazon.com/Amazon-Basics-Uni-Directional-DisplayPort-Display/dp/B015OW3M1W) are fine.  

If you need an active Displayport to HDMI adapter, buy one from a reputable vendor. We recommend [Club3D 1085](https://www.amazon.com/Club-3D-DisplayPort1-4-Adapter-CAC-1085/dp/B08BX49V5V) for 4K@120Hz. [Club3D 1080/1082/2070](https://www.amazon.com/CLUB-3D-CAC-1082-Active-Adapter/dp/B07HNTNTMR), [Monoprice](https://www.amazon.com/Monoprice-DisplayPort-1-2a-Active-Adapter/dp/B07FPQ4ZSW), [UPTab](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) or [Plugable](https://www.amazon.com/Plugable-DisplayPort-Supports-displays-3840x2160/dp/B00S0C7QO8) for 4K@60Hz.  

If you need a USB-C to HDMI adapter, we recommend Cable Matters [Adapter](https://www.amazon.com/Cable-Matters-Braided-Adapter-Aluminum/dp/B08KSMK87K)/[Cable](https://www.amazon.com/Cable-Matters-USB-C-Supporting-Black/dp/B073H9RG9T) for 4K@60Hz and Cable Matters [Adapter](https://www.amazon.com/dp/B08MSWMXT4)/[Cable](https://www.amazon.com/dp/B08QDV5H4M) for up to 4K@120Hz.  

<!-- Sub-Section -->

### Keyboards/Remotes/Gamepads

It's highly recommended that you do NOT put 2.4 Ghz wifi routers in the same room as RF or BT devices below.  

For **keyboards**, one with an integrated trackpad and backlight for use in the dark is ideal, but a premium one (like the Logitech K830 or Corsair K83) is hard to find. Logitech and Microsoft will be the most supported and of higher quality. If you want specific features, you may be forced to venture out to Riitek, Arteck or other unknown sellers. Do not expect the highest quality or good support.  
RF and Bluetooth (BT) are the most used connection technologies. Use either with a HTPC. For media devices/smart tvs, BT will be most supported  

KEYBOARD						|	PRICE	|	SIZE	|	INT		|	BACKLIT	|	POINT	|	BATTERY	|	NOTES
:--|:--|:--|:--|:--|:--|:--|:--|
[Logitech K830](https://www.logitech.com/en-us/products/keyboards/k830-illuminated-tv-wireless.html)				|	[Disc (1)](https://www.amazon.com/dp/B00ZOPVSKW?ref=emc_p_m_9_b&th=1)	|	Full	|	BT/RF	|	Yes		|	Pad		|	Int		|	14.4", [Ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=logitech+k830&_sacat=0)
[Logitech K400](https://m.media-amazon.com/images/I/A1-V3Jgn7ZL.pdf)				|	[$30](https://www.amazon.com/Logitech-Wireless-Keyboard-Multi-Touch-Touchpad/dp/B005DKZTMG)		|	Full	|	RF		|	No		|	Pad		|	AA		|	14"
**[Logitech K400 Plus](https://www.logitech.com/en-us/products/keyboards/k400-plus-touchpad-keyboard.html)**		|	[$20](https://www.amazon.com/Logitech-Wireless-Keyboard-Touchpad-PC-connected/dp/B014EUQOGK)		|	Full	|	RF		|	No		|	Pad		|	AA		|	14", dual Fn keys
[Logitech K600](https://www.logitech.com/en-us/products/keyboards/k600-smart-tv-d-pad.920-008822.html)				|	[$70](https://www.amazon.com/Logitech-K600-TV-Keyboard-Integrated/dp/B07C6LXYHL)		|	Full	|	BT/RF	|	No		|	Pad		|	AAA		|	14.4", D-pad
[Microsoft All-In-One Media](https://www.microsoft.com/en/accessories/products/keyboards/all-in-one-media-keyboard)	|	[$40](https://www.microsoft.com/en-us/d/microsoft-all-in-one-media-keyboard/8ttd9j9jnsf0)		|	Full	|	RF		|	No		|	Pad		|	AAA		|	14.4", [Amazon](https://www.amazon.com/s?k=microsoft+all+in+one+keyboard&rh=n%3A172282%2Cp_89%3AMicrosoft)
[Arteck B08SK8D38P (HD197)](https://www.google.com/search?q=arteck+hd197)	|	[$30](https://www.amazon.com/dp/B08SK8D38P)		|	Full	|	BT		|	No		|	Pad		|	Int		|	14.6", multi-connection
**[Arteck HB305-4B](https://www.google.com/search?q=arteck+hb305+4b)**			|	[$35](https://www.amazon.com/dp/B09KLPJQPD)		|	Full	|	BT		|	Yes		|	Pad		|	Int		|	14.2"
[Rii K22/K22-BT](https://riitek.com)				|	[$25/$32](https://www.amazon.com/Rii-K22-Multimedia-Rechargable-Raspberry/dp/B07KPVZ1Y4)	|	Full	|	RF/BT	|	No		|	Pad		|	Int		|	14", multi-connection (BT)
[Coastacloud B09PXYG3X7](https://www.amazon.com/stores/page/4040CD3A-98E3-48AF-BF5E-12F0EF68349C?ingress=2&visitId=2bbe211d-642b-4dc5-b467-bf026e93b00b&ref_=ast_bln)		|	[$42](https://www.amazon.com/dp/B09PXYG3X7)		|	Full	|	RF/BT	|	Yes		|	Pad		|	Int		|	14.4", generic
[Rii K18+](http://www.riitek.com/product/226.html)				|	[$27](https://www.amazon.com/Rii-Wireless-Keyboard-Rechargable-Raspberry/dp/B077VYRMC1)		|	Full	|	RF		|	Yes		|	Pad		|	Int		|	12.8"
**[Rii RT518S](https://www.amazon.com/Rii-Wireless-Keyboard-Rechargable-Raspberry/dp/B092CL5PNN/)**				|	[$35](https://www.amazon.com/Rii-Wireless-Keyboard-Rechargable-Raspberry/dp/B092CL5PNN/)		|	Full	|	RF/BT	|	Yes		|	Pad		|	Int		|	12.8". Version of K18+
[Lenovo TrackPoint II](https://www.lenovo.com/us/en/p/accessories-and-software/keyboards-and-mice/keyboards/4y40x49493)		|	[$120](https://www.amazon.com/Lenovo-ThinkPad-TrackPoint-Keyboard-4Y40X49493/dp/B08BWQXZYL)	|	Compact	|	RF/BT	|	No		|	Nub		|	Int		|	12"
[XIWMIX Ultra-Slim Touchpad Keyboard](https://www.amazon.com/dp/B0B9SLXMCC/?th=1)	|[$40](https://www.amazon.com/dp/B0B9SLXMCC/?th=1)	| Compact | BT | Yes | Pad | Int | 9.7"
[Macally BTTVKEY](https://www.amazon.com/Macally-BTTVKEY/dp/B08S3S6ZDV)				|	[$30](https://www.amazon.com/Macally-BTTVKEY/dp/B08S3S6ZDV)		|	Compact	|	BT		|	No		|	Pad		|	AAA		|	9.7"
Rii [K12+](https://www.amazon.com/Rii-K12-Portable-Stainless-Rechargeable/dp/B011KPIZ9G)					|	[$30](https://www.amazon.com/Rii-K12-Portable-Stainless-Rechargeable/dp/B011KPIZ9G)		|	Compact	|	RF		|	No		|	Pad		|	Int		|	10"
[Logitech DiNovo Mini](https://download01.logitech.com/web/ftp/pub/pdf/keyboards/diNovo_productguide_eng-fre.pdf)		|	[Disc (1)](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=dinovo+mini&_sacat=0)	|	Mini	|	BT/RF	|	Yes		|	Pad		|	Prop (2)|	6", [Ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313&_nkw=dinovo+mini&_sacat=0)
[Rii i4](http://www.riitek.com/product/i4.html)						|	[$30](https://www.amazon.com/dp/B07T13GLY3)		|	Mini	|	RF/BT	|	Yes		|	Pad		|	Int		|	6"
**[Rii i8+/i8+ BT](http://www.riitek.com/plus/search.php?kwtype=0&searchtype=titlekeyword&keyword=i8)**				|	[$30](https://www.amazon.com/Rii-Bluetooth-Touchpad%EF%BC%86QWERTY-Smartphones-Raspberry/dp/B01GCPVZDW)		|	Mini	|	RF/BT	|	Yes		|	Pad		|	Int		|	5.8"
[Rii K06BT](http://www.riitek.com/product/k06bt.html)/X1BT					|	[$30](https://www.amazon.com/Wireless-Bluetooth-Touchpad-Keyboard-Android/dp/B07FRBMS12)/[$30](https://www.amazon.com/dp/B07TS7TQ8J)		|	Micro	|	BT		|	Yes		|	Pad		|	Int		|	5.8"
[Rii i15](http://www.riitek.com/product/i15.html)						|	Disc? (1)		|	Micro	|	RF/BT	|	Yes		|	Pad		|	Int		|	5.3"
[Rii - Various](http://www.riitek.com/product/mini.html)				|	NA		|	Various	|	RF/BT	|	Various	|	Various	|	Int		| All others
[Perixx trackball keyboards](https://perixx.com/collections/keyboards?pf_t_features=features%3A+Trackball&pf_t_features_and_condition=true)	| [$25-$150](https://www.amazon.com/s?k=perixx+keyboard+trackball&i=electronics&crid=2YKIEQC3WUT5S&sprefix=perixx+keyboard+trackball%2Celectronics%2C140&ref=nb_sb_noss_1)	|	Various	|	USB/RF	|	Various		|	Ball		|	Various		|	9"-18.6"
No-name trackball keyboards	| [$35](https://www.amazon.com/dp/B094VVL7Q9)/[$45](https://www.amazon.com/dp/B076HNGH9Q)	|	Compact/Full	|	RF	|	No		|	Ball		|	AA		|	10.2"/14.1"

(1) Discontinued  
(2) Proprietary, removable, can be replaced  

For **remotes**, the [Logitech Harmony](https://www.logitech.com/en-us/harmony-universal-remotes) series is the Rolls Royce of remotes, but is now discontinued, so look on the secondary market. The [Sofabaton](https://www.sofabaton.com/) is a decent replacement for it. Everything below those are the lower tier and under $50. The [WeChip G20S Pro](https://www.amazon.com/WeChip-Backlight-Wireless-Replacement-Protector/dp/B08VN98V93) remote is simple and backlit. The [Pepper Jobs W10](https://www.amazon.com/W10-GYRO-Keyboard-Controller-Learning/dp/B078NT49MJ) remote has a bunch of PC specialized keys on it. The MX3 Pro is less specialized but still has air mouse functionality, a keyboard and is backlit. There is no shortage of other bluetooth and RF based remotes floating around, depending on which buttons, form factor and price you're shooting for.  

REMOTE			|	PRICE	|	INT		|	BACKLIT	|	BATTERY	|	NOTES
:--|:--|:--|:--|:--|:--|
Logitech Harmony One	|	Disc (1)	|	RF/BT/IR	|	Yes	|	Int	|	IR Blaster, Hub
Sofabaton U1		|	$50	|	BT/IR		|	NO	|	AA	|	NA
Sofabaton X1		|	$190	|	BT/IR (Hub)	|	Yes	|	Int	|	IR Blaster, Alexa
**[Pepper Jobs W10](https://www.pepper-jobs.com/products/w10-gyro-smart-remote)**		|	$30	|	RF/IR		|	Yes	|	AAA	|	Has mini keyboard
WeChip G20S Pro		|	$20	|	RF		|	Yes	|	AAA	|	BT in Pro Plus
MX3 Pro			|	$20	|	RF		|	Yes	|	AAA	|	NA
[HTWebRemote](https://github.com/nicko88/HTWebRemote)	|	Free	|	LAN		|	NA	|	NA	|	Software to create web-accessible remote on Windows/[Linux](https://github.com/nicko88/HTWebRemoteHost) HTPC to control multiple devices. [Contact](https://www.reddit.com/message/compose/?to=SirMaster)
[Unified Remote](https://www.unifiedremote.com/)	|	Free/$5	|	LAN		|	NA	|	NA	|	Software to create app-accessible remote on Windows/Linux HTPC to control multiple devices
[DS4Windows](https://ds4-windows.com/)	|	Free	|	NA		|	NA	|	NA	|	Software to use DS3/DS4/DS5 controllers as mouse/remote
[JoyXOff](https://joyxoff.com/en/)	|	Free	|	NA		|	NA	|	NA	|	Software to use Xbox/XInput controllers as keyboard/mouse/remote
[Netflix Remote Controller](http://sticky-ux.com/apps/NetflixRemoteController/)		|	Free	|	NA		|	NA	|	NA	| Software to control Windows Netflix app from keyboard/remote

(1) Discontinued  

If you already have an IR remote, you can use a [Flirc](https://flirc.tv/more/flirc-usb) adapter to allow it to be used with your HTPC and/or Nvidia Shield. Flirc also makes a programmable IR remote, the [Skip 1s](https://flirc.tv/products/skip1s-remote?variant=43489094729960#Overview)  

For **gamepads**, look at [8bitdo](https://www.8bitdo.com/) or Microsoft for highly-compatible Xbox wireless controllers. For multi-user play, you can pair multiple Xbox controllers with a single USB adapter or 2-4 regular BT controllers with a single [USB BT adapter](https://www.amazon.com/IOGEAR-Bluetooth-Multi-Language-Version-GBU521W6/dp/B007ZT2AXE) (CSR8510/BCM20702 chipsets)  

To get HDMI-CEC functionality where none exists, use a [Pulse Eight](https://www.pulse-eight.com/p/104/usb-hdmi-cec-adapter) adapter.  

To transmit IR from your HTPC to other devices, use a [USB-UIRT](http://www.usbuirt.com/).  

On the software side, [Plex HTPC](https://support.plex.tv/articles/plex-htpc-input-maps/), [Kodi](https://kodi.wiki/view/Remote_controls), and [Jriver Media Center](https://wiki.jriver.com/index.php/Remotes) all support multiple remote types. You can also use [AutoHotKey](https://www.autohotkey.com/) and/or [EventGhost](http://www.eventghost.net/) to automate keyboard tasks.  

<!-- Section -->

## How do i wake/power on/power off my HTPC with a remote/mobile app?

You may want to wake your HTPC from sleep or have the ability to power it on or off from your remote control or a mobile app. There are a few ways to do this. Each has its own pros and cons.  

1. Wake: Use a [Flirc USB](https://flirc.tv/more/flirc-usb) device plugged into your HTPC and an IR remote

2. Wake/Power On/Off: Use a [Flirc Streamcom USB](https://flirc.tv/products/flirc-streacom?variant=43085036486888) device wired into your HTPC mobo and an IR remote. Requires a case with an IR window or drill-modded to allow the IR signal into the module.

3. Wake: Use a HTPC with an IR sensor ([Intel NUC 7/8/11, Asus PN, Gigabyte Brix](/htpc-wiki/nuc)) and a [Pepper Jobs W10](https://www.pepper-jobs.com/products/w10-gyro-smart-remote) IR remote

4. Wake/Power On/Off: Use a Silverstone [ES02](https://www.silverstonetek.com/en/product/expansion-cards/?page=1&filter=Power_OnOff_addon_cards&sort=Newsest) and included remote or [ES03-WIFI](https://www.silverstonetek.com/en/product/expansion-cards/?page=1&filter=Power_OnOff_addon_cards&sort=Newsest) and mobile app

5. Power On/Off: Use a [Simerec IR Remote Switch](https://www.simerec.com/index.html) and an IR remote  

6. Power On/Off: Plug your HTPC into a [smart power plug](https://www.amazon.com/Assistant-Controlled-Google-Enabled-Vacation/dp/B07XZT24B8). Use with mobile app and/or google/alexa voice tech. If you're IoT-averse, use a [dumb power plug](https://www.amazon.com/DEWENWILS-Control-Wireless-Interference-Programmable/dp/B09X2W2TRT) w/remote instead.

7. Power On/Off: Plug your HTPC into a [power strip with a master/control](https://www.amazon.com/Smart-Strip-LCG-3MVR-Autoswitching-Technology/dp/B0006PUDQK/ref=psdc_761520_t1_B01G6VTIDG) plus and configure your BIOS to set Power On for AC after power loss. Plug master/initial power-on device (like TV) into control port.

8. Wake/Power On: [Configure Wake-on-Lan](https://www.gearrice.com/update/turn-on-a-pc-remotely-with-wake-on-lan-or-remote-control/) in your BIOS and on your network card. Use with a mobile app like Unified Remote

9. Wake/Power On/Off: Install a [SwitchBot bot](https://www.switch-bot.com/) on your HTPC's power button. Use SwitchBot Remote or mobile app.

10. Wake: Use HDMI CEC with another HT device


## Why would I use a PC over a media device (roku, firetv, shield, etc..) for a HTPC?

While media devices are great frontends that are easy to use and navigate, they're not for every scenario. They are best when your usage profile is limited, esp. in terms of the software and hardware you want to use. These are a lot of the reasons you may want to use a PC for your HTPC instead of a media device.  

1. You want to run apps/services on windows or linux, or use a specific, customizable interface, that is/are not available on media device operating systems.  

2. You want to do moderate to extensive web browsing. Media devices, while they can do it, are not good at this from both a HTML spec perspective and for ease of navigation.  

3. You want it to function as a server. You want to provide services like sonarr, radarr, tautulli, plex, VMs, bittorrent.  

4. You want to have more control over video processing; with video renderers like madVR and SVP you can have more control and get better results when doing things like HDR->SDR tonemapping and image, chroma and frame-rate upscaling. You want video refresh rates beyond 60 Hz (e.g. 120 Hz). You need to use multiple displays.  

5. You want more control over audio processing (decoding, mixing, equalization, etc..). You want HD audio (TrueHD, Atmos) that most streaming devices don't provide. Most streaming devices like Roku, FireTV (some), Chromecast (not counting Nvidia Shields or SBCs) don't provide HD audio. They'll only do lower quality versions of DD/DTS/Atmos. See media devices section below for details per device.  

6. You'd rather use a keyboard/mouse instead of a remote for navigation. Media devices are better suited for remote-based navigation. PCs are better suited for keyboard/mouse.  

7. You want to combine HTPC and other computing duties into one machine and/or you don't want to maintain more than one device.  

8. You need more processing power than a streaming device can provide (Local gaming, emulation gaming >= GameCube, VR, etc..)  

9. You like to build things. You'd rather use commodity/DIY hardware/software.  

10. You need more I/O ports or more of a variety of ports (USB, optical, gigabit LAN, 3.5" audio etc..) than most media devices provide and would rather not buy external hardware to do this. You plan to use hardware not supported on a streaming device (USB DAC, TV tuner card. sound card, etc..)  

11. You want to have internal storage rather than external storage.  

12. You have privacy concerns with proprietary systems.  


## What software will I need and how do I set it up?

For the software side of things, there are various tools you may need to take advantage of your HTPC. An OS, media player, media server, ripper, downloader, file renamer, etc.. [This page](http://kodi.wiki/view/Supplemental_tools) has a list of supplemental software relating to HTPCs.

**Operating Systems:** 

At the minimum you'll need an OS. Windows, Linux and Android are the most popular choices, as you can imagine. If you want to get the highest resolution from streaming services (esp. DRMed ones), use HDR, video upscaling like madVR, or are combining with a gaming solution, you would use Windows. Alternatively, using Linux is possible, but you will be limited to [lower resolution streaming services](/htpc-wiki/faq#what-resolution-is-supported-on-streaming-service-x) and no HDR. There are some specialized OSes out there, like [LibreElec](https://libreelec.tv/)/[CoreElec](https://coreelec.org) which are OSes designed for just running a media player (Kodi) with a single, plugin-capable interface. They also suffer from lower resolutions on streaming services but are very good for local content, even HDR.  

**Media Players:** 

For [video streaming services](/htpc-wiki/faq#what-resolution-is-supported-on-streaming-service-x), use Microsoft Edge to get 1080p+, or the service's app (if available).  

For simple media players, using local content, [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases), [VLC](https://www.videolan.org/vlc/) and Pot Player are popular on Windows, with [VLC](https://www.videolan.org/vlc/) on Linux.  

If [HDR passthrough](/htpc-wiki/hdr) is what you're looking for, then look at [MPC-BE](https://github.com/Aleksoid1978/MPC-BE/releases), [VLC](https://www.videolan.org/vlc/) or Kodi. For high-end video upscaling or HDR tonemapping, look at getting the [madVR](http://madvr.com) renderer for MPC-BE, Kodi, or Potplayer. For FPS upscaling, [SmoothVideo Project](https://www.svp-team.com/).  

But perhaps you want a more full-featured player/interface..  

If you DON'T need to serve media to other devices and just want a well-supported, highly-customizable home theater front-end, look at [Mediaportal](http://www.team-mediaportal.com/), [Jriver](https://www.jriver.com/) or [Kodi](http://kodi.tv/). All three will pull down metadata for the media you point them to, keep track of what you have watched/haven't watched, keep playback progress, pass-through HDR, and play from your internal or network storage. For Kodi, start with Kodi's [First Time User guide](https://kodi.wiki/view/First_time_user) and 3rd party guides like [this](https://androidpcreview.com/how-to-setup-kodi-the-right-way/). For the others, venture over to their subreddit or forums for setup help.  

**Media Servers:** 

If you DO need to serve media to other devices (local or remote), [Plex Media Server](https://www.plex.tv) is very popular and will index your media, pull metadata (like cover art/plot/cast/tv show data), track what you have watched/haven't watched and stream it out to your client devices. It also has a [wide range of player apps](https://www.plex.tv/media-server-downloads/#plex-app) to install on your client devices. For PC specifically, there is Plex HTPC (keybrd/remote-based) and Plex for Windows (mouse-based). If you don't like the plex-branded ones, you can, alternatively, integrate the [Kodi](https://kodi.tv/addons/matrix/script.plex) player with the Plex server. For an alternative to Plex Media Server, there is [Emby](http://emby.media/). Emby is an open-source product. Like Plex, it can stream media to many different platforms.  

**Launchers:** 

For a launcher interface to open multiple apps, look at [Flex Launcher](https://github.com/complexlogic/flex-launcher) (Windows/Linux), [Steam Big Picture mode](https://store.steampowered.com/bigpicture) (Windows/Linux/Mac), [Windows 10 start menu in full screen mode](https://www.reddit.com/r/htpc/comments/92ek4d/homescreen_for_htpc_and_ideas_for_what_i_can_put/e356duu/), [Windows tablet mode](https://www.tenforums.com/tutorials/3755-turn-off-tablet-mode-windows-10-a.html), or [customize Kodi](https://kodi.wiki/view/Archive:HOW-TO:Make_Windows_boot_directly_to_Kodi_\(as_a_shell\)) and use [add-ons/favorites](https://kodi.wiki/view/Favourites).  

**Organization:** 

To organize your content, look at Radarr (movies), Sonarr (tv), Lidarr (music) and Bazarr (subtitles). You can use these together to keep your content in properly named files/folders for Plex, retrieve subtitles and show you what content you have or don't have. You can interface with these using their respective web interfaces or with an app like [nzb360](https://play.google.com/store/apps/details?id=com.kevinforeman.nzb360&hl=en_US&gl=US) on an android device. For metadata management, look at [Media Hoarder](https://media.hoarder.software). For file management, look at [Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) [w/LAN plugin](https://play.google.com/store/apps/details?id=com.ghisler.tcplugins.LAN) or [X-Plore](https://www.lonelycatgames.com/apps/xplore).  

**Other software:** 

For Live TV software, see the [dedicated section](/htpc-wiki/faq#can-i-watch-live-tv-or-record-it-and-play-it-back-on-my-htpc) below.  

For blu-ray disc playback, both Kodi and VLC (w/[Java 8](https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html)) have disc menu support ; for 4k/UHD, use [Cyberlink PowerDVD](https://www.cyberlink.com/products/powerdvd-ultra/features_en_US.html)  

For disc ripping and transcoding software, see the [dedicated section](/htpc-wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use) below.  

For game emulation, look at [RetroArch](https://www.retroarch.com/?page=platforms), [EmulationStation DE](https://es-de.org/) or [Launchbox Big Box](https://www.launchbox-app.com/premium) on **Windows**. [Batocera](https://batocera.org/), [Lakka (RetroArch on a stick)](https://www.lakka.tv/) on **Linux**, RetroArch or [OpenEmu](https://openemu.org/) on **Mac**, [Lemuroid](https://play.google.com/store/apps/details?id=com.swordfish.lemuroid&hl=en_US&gl=US) or RetroArch on **Android**, [Provenance](https://github.com/Provenance-Emu/Provenance) on **Apple TV**. [Nostlan](https://github.com/quinton-ashley/nostlan) for 4k displays.  

For game streaming, [Sunshine](https://app.lizardbyte.dev/Sunshine) on your server/gaming PC and [Moonlight](https://moonlight-stream.org/) on your client.  

For an overall sense of how a basic HTPC platform should look with playback, serving, storage, and organization, look at our [diagram here](https://i.imgur.com/gUI1R6z.png).  

If you're planning on replacing cable/sat with similar streaming services, you will find [r/cordcutters](https://www.reddit.com/r/cordcutters/) to be helpful.  

If you'd like to have a podcast, audio podcast or audiobook library in Plex, [see this handy guide](http://www.reddit.com/r/PleX/comments/3avpi9/how_to_create_a_podcast_library_a_video_podcast/).  

For a comprehensive guide to setting up all the backend organizational/serving software, we can recommend [The Ultimate Server Guide](http://www.cuttingcords.com/home/ultimate-server/getting-started). This guide takes you through Sonarr, Couchpotato, Headphones, Deluge, SabNZBd and [Plex Media Server](https://plex.tv/). The [htpc box guide](https://github.com/sebgl/htpc-download-box) will take you through a more modern installation approach to the stack using Docker containers. The [Servarr Wiki](https://wiki.servarr.com/) is a great reference for all the \*arr software.  


## Can I use my HTPC for streaming from services such as Netflix, Youtube, Amazon, Hulu, etc..? 

Yes, however the interface quality and functionality varies widely and remote control support is almost non-existent. The services will detect your device as a PC and present you with their standard web or app-based interface. It may be up to you to start videos and expand them to full-screen.  

If you don't plan on using a [keyboard/mouse-like device](/htpc-wiki/faq#keyboardsremotesgamepads), then streaming services on a PC will be painful. There are some workarounds like [software](/htpc-wiki/faq#keyboardsremotesgamepads) to emulate a mouse on game controllers/mobile and things like the [Leanback interface](https://redd.it/y5o7mi) for Youtube. If those things aren't good enough for you, then you should buy a remote-based [media device](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) from the next section instead.  

Using Windows Store apps for some of these services may be better than using a web browser in terms of video/audio support. 

For example, the Netflix Windows Store app does support 4k/1080p streaming and Dolby Digital/Dolby Digital Plus soundtracks. Browser-based solutions tend not support DD/DD+ audio and some content will only be available in 720p. The app still does not have remote control support, but you can try adding 3rd party remote control support using the [Netflix Remote Controller](http://sticky-ux.com/apps/NetflixRemoteController/).  

4K support for streaming services in general is limited on a traditional HTPC. See our sections on [streaming service resolutions supported](/htpc-wiki/faq#what-resolution-is-supported-on-streaming-service-x) and [4K compatibility](/htpc-wiki/faq#what-do-i-need-for-4k-ultrahd-compatibility) below.  

Support for the higher resolutions and audio is way more prevalent on pre-built media devices, so if you use a lot of these services, it's better not to use a PC. Again, see our [media device](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) section below.  

In regards to bandwidth required, you should have 6 Mbps downstream to stream 1080p services. 25 Mbps for 4k.  


## Can I use a pre-built media device for my HTPC?

Yes, you can. There are many already-built devices out there. Media devices from major brands like Roku/Amazon/Google/Apple/Nvidia/Roku will have better support for video resolutions/HDR than a traditional HTPC. See the next section for why you would choose one device or brand over another. There is also a list of popular devices at [wikipedia](https://en.wikipedia.org/wiki/Comparison_of_digital_media_players) which gives further information like supported streaming apps.  

Beware of cheap no-name android boxes on obscure websites. They likely will have no or poor support and very little documentation if you run into trouble.  

If you're looking for the best Plex client, watch [this](https://www.youtube.com/watch?v=qLxjL2NxZy8) video for tests on loading/scrolling/playing/audio/remotes/etc..  

If you want a traditional standalone HTPC see the Mini PCs at the end of the list or our [Sample Builds](/htpc-wiki/sample-builds) page for more extensive options.  

Legend: PT: Passthrough, DC: Decode, LS: Lossy, LL: LossLess, DD: Dolby Digital, DV: Dolby Vision, DA: Dolby Atmos, DTHD: Dolby TrueHD, EOL: End of Life

BRAND/MODEL|PRICE|RESOLUTION|4k NETFLIX?|HDR?|WIFI?|LAN?|VOICE SEARCH?|USB?|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
[Raspberry Pi 4b](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/) ([buy](https://www.pishop.us/product/raspberry-pi-4-model-b-1gb/))|$36|4k@60 (2)|No|YES (2)|ac|1000M|No|YES (8b)|HDR10/HLG, LL DTHD/DTS-HD, BT 5.0
[Raspberry Pi 5](https://www.raspberrypi.com/products/raspberry-pi-5/) ([buy](https://www.pishop.us/product/raspberry-pi-5-4gb/))|$60|4k@60 (4)|No|YES (2)|ac|1000M|No|YES (8b)|HDR10/HLG, LL DTHD/DTS-HD, BT 5.0
[Odroid C4](https://www.hardkernel.com/shop/odroid-c4/) ([buy](https://www.hardkernel.com/shop/odroid-c4/))|$55|4k@60|No|YES (6)|Opt|1000M|No|YES (8b)|S905X3/4GB RAM. HDR10, PT:LL DA/DTSX w/CoreElec
[Odroid N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ([buy](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/))|$66|4k@60|No|YES (6)|Opt|1000M|No|YES (8b)|S922x/2GB RAM/8 GB SD. HDR10, PT:LL DA/DTSX w/CoreElec
[Dune HD Box R Plus](https://www.dune-hd.com/products/homatics-box-r-4k-plus) ([buy](https://www.dune-hd.com/products/homatics-box-r-4k-plus))|$150|4k@60|No|YES (6)|ax|1000M|No|YES (8b)|S905X4-K/4GB RAM/32 GB SD. HDR10+/DV-5/7/8, PT:LL DA/DTSX w/CoreElec
[Mi Box S](https://www.mi.com/global/mi-box-s) ([buy](https://www.amazon.com/Xiaomi-Android-Google-Assistant-Streaming/dp/B07KLWGGYS))|$65|4k@60|YES|YES|ac|No|YES|YES (8b)|BT 4. HDR10, PT:LS DD+/DTS, S905X-H/2GB/8GB
[Apple TV 4k (2021)](https://www.apple.com/apple-tv-4k/) ([buy](https://www.apple.com/shop/buy-tv/apple-tv-4k))|$179/$199|4k@60|YES|YES|ax|1000M|YES|No|2nd gen, A12, 3GB/32-64GB, HDR10/DV-5, DC:DTHD/DTSHD->PCM, PT:LS DA, BT 5.0
**[Apple TV 4k (2022)](https://www.apple.com/apple-tv-4k/)** ([buy](https://www.apple.com/shop/buy-tv/apple-tv-4k))|$129/$149|4k@60|YES|YES|ax|1000M (7)|YES|No|3rd gen, A15, 3GB/64-128GB, HDR10+/DV-5, DC:DTHD/DTSHD->PCM, PT:LS DA, BT 5.0
[ChromeCast w/Google TV HD](https://store.google.com/product/chromecast_google_tv) ([buy](https://store.google.com/product/chromecast_google_tv))|$30|1080p|No|YES|dual ac|Opt|YES|Opt (8a)|HDR10+, AV1, DC:DD+, PT:LS DA/DTS, S805X2, 1.5GB/8GB
**[ChromeCast w/Google TV 4k](https://store.google.com/product/chromecast_google_tv)** ([buy](https://store.google.com/config/chromecast_google_tv))|$50|4k@60|YES|YES|dual ac|Opt|YES|Opt (8a)|2nd/latest gen. Remote, HDR10+/DV, DC:DD+, PT:LS DA/DTS, BT 4.1, S905D3 1.9Ghz/2GB/8GB
**[Amazon Fire TV stick 4K MAX (2023)](https://www.amazon.com/dp/B0BP9SNVH9)** ([buy](https://www.amazon.com/dp/B0BP9SNVH9))|$60|4K@60|YES|YES|tri ax 2x2-6e|Opt (9)|YES|Opt (8a)|2nd gen, BT 5.2 LE, AV1, HDR10+/DV, PT:LL DA/DTSHD, 2.0Ghz/2GB/16GB
[Amazon Fire TV stick 4K MAX (2021)](https://www.amazon.com/dp/B08MQZXN1X) ([buy](https://www.amazon.com/dp/B08MQZXN1X))|$55|4K@60|YES|YES|dual ax 2x2-6|Opt (9)|YES|Opt (8a)|1st gen, BT 5.0 LE, AV1, HDR10+/DV, PT:LS DA, 1.8Ghz/2GB/8GB
[Amazon Fire TV stick 4K (2023)](https://www.amazon.com/dp/B0CDR2MSVC) ([buy](https://www.amazon.com/dp/B0CDR2MSVC))|$50|4K@60|YES|YES|dual ax 2x2-6|Opt (9)|YES|Opt (8a)|2nd gen, BT 5.2 LE, HDR10+/DV-4/5/8/9/10, PT:LL DA, 1.7Ghz/2GB/8GB
[Amazon Fire TV stick 4K (2018)](https://www.amazon.com/all-new-fire-tv-stick-4k-with-alexa-voice-remote/dp/B08XVYZ1Y5) ([buy](https://www.amazon.com/all-new-fire-tv-stick-4k-with-alexa-voice-remote/dp/B08XVYZ1Y5))|$45|4K@60|YES|YES|dual ac 2x2|Opt (9)|YES|Opt (8a)|1st gen, BT 5.0 LE, HDR10+/DV, PT:LS DA, 1.7Ghz/1.5GB/8GB
[Amazon Fire TV stick](https://smile.amazon.com/dp/B07ZZVX1F2/) ([buy](https://smile.amazon.com/dp/B07ZZVX1F2/))|$40|1080p|NO|YES|dual ac 2x2|Opt (9)|YES|Opt (8a)|3rd Gen, BT 5.0 LE, HDR10+, DC: LS DA, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[Amazon Fire TV stick Lite](https://smile.amazon.com/dp/B07YNLBS7R/) ([buy](https://smile.amazon.com/dp/B07YNLBS7R/))|$30|1080p|NO|YES|dual ac 2x2|Opt (9)|YES|Opt (8a)|BT 5.0 LE, HDR10+, PT:LS DA/DTS, 1.7Ghz/1GB/8GB
[Amazon Fire TV cube](https://smile.amazon.com/All-new-hands-free-Alexa-streaming-player/dp/B07KGVB6D6) ([buy](https://smile.amazon.com/All-new-hands-free-Alexa-streaming-player/dp/B07KGVB6D6))|$140|4K@60|YES|YES|tri ax 2x2-6E|10/100 (9)|YES|YES (8b)|3rd gen, BT 5 LE, AV1, HDR10+/DV, PT:LL DA/DTSHD,DC:LL DA->PCM, 2.2Ghz/2GB/16GB
[Roku Express](https://www.roku.com/products/roku-express)/[+](https://www.roku.com/products/roku-express-plus) ([buy](https://smile.amazon.com/Roku-Express-Streaming-Media-Player/dp/B07WVFCVJN)/[buy+](https://www.walmart.com/ip/Roku-Express-Streaming-Media-Player-2019/799113308))|$25/$30|1080p|NO|No|n|No|No/YES|No|DD, PT:LS DTS/DA
[Roku Express+ (2017)](https://www.roku.com/products/roku-express-plus) ([buy](https://smile.amazon.com/Roku-Express-HD-Streaming-Player/dp/B01LXJA5JD))|$40|1080p|NO|No|n|No|No|No|Has composite cable
[Roku Express 4K](https://www.roku.com/products/roku-express-4k)/[+](https://www.roku.com/products/roku-express-4k-plus) ([buy](https://www.walmart.com/ip/Roku-Express-4K-2021-Streaming-Media-Player-HD-4K-HDR-with-Smooth-Wireless-Streaming-and-Simple-Remote-includes-Premium-HDMI-Cable/651641821)/[buy](https://amzn.to/3g56Djl))|$35/$40|4k@60|YES|YES|dual ac|No/Opt|No/YES|Opt|HDR10+, DC:DD/PT:LS DTS/DA
**[Roku Streaming 4K](https://www.roku.com/products/roku-streaming-stick-4k)** ([buy](https://www.amazon.com/Roku-Streaming-Device-Vision-Controls/dp/B09BKCDXZC))|$40|4k@60|YES|YES|dual ac 2x2|No|YES|No|1GB, DV/HDR10+, DC:DD/PT:LS DTS/DA. Model: 3820R
[Roku Streaming 4K+](https://www.roku.com/products/roku-streaming-stick-4k-plus) ([buy](https://www.amazon.com/dp/B09BKCQYRN?ref=emc_p_m_5_i))|$70|4k@60|YES|YES|dual ac 2x2|No|YES|No|1GB, DV/HDR10+, DC:DD/PT:LS DTS/DA. Model: 3821R
[Roku Ultra](https://www.roku.com/products/roku-ultra) ([buy](https://www.bhphotovideo.com/c/product/1594956-REG/roku_4800r_ultra_streaming.html))|$100|4k@60|YES|YES|dual ac|100M|YES|YES (8b)|2GB RAM, HDR10+/DV, DC:DA, PT:LS DTS/DA, BT. AV1. Model: 4800R
[Roku Ultra LT](https://www.roku.com/products/roku-ultra-lt) ([buy](https://www.walmart.com/ip/Roku-Ultra-LT-Streaming-Media-Player-2019/857445471))|$80|4k@60|YES|YES|dual ac|100M|YES|No|2GB RAM, HDR10, DC:DD+, PT:LS DTS/DA. Model: 4801RW
[Vero 4K+](https://osmc.tv/vero/) ([buy](http://buy.getvero.tv/))|$140|4k@60|No|YES|ac|1000M|No|YES (8b)|OSMC, BT 4.0, HDR10, PT:LL DA/DTSX, 1.6Ghz/2GB/16GB
[Nvidia Shield TV Tube](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP94PBJ))|$150|4k@60|YES|YES|ac|1000M|YES|No|DV-5/8/HDR10, PT:LL DA/DTSX DC:DA, 2GB/8GB, BT 5, microSD
**[Nvidia Shield TV Pro](https://www.nvidia.com/en-us/shield/shield-tv-pro/)** ([buy](https://smile.amazon.com/NVIDIA-Shield-Streaming-Player-Performance/dp/B07YP9FBMM))|$199|4k@60|YES|YES|ac|1000M|YES|YES (8b)|DV-5/8/HDR10, PT:LL DA/DTSX DC:DA, 3GB/16GB, BT 5
[Nvidia Shield TV (2017)](https://www.nvidia.com/en-us/shield/shield-tv/) ([buy](https://smile.amazon.com/NVIDIA-SHIELD-Gaming-Streaming-GeForce/dp/B075RXV2VR))|$179|4k@60|YES|YES|ac|1000M|YES|YES (8b)|HDR10, PT:LL DA/DTSX, 16GB
[Xbox One S/X](https://www.xbox.com/en-US/xbox-one/consoles) ([buy](https://smile.amazon.com/gp/bestsellers/electronics/6469295011))|$200-$400|4k@60|YES|YES|dual-ac|1000M|No|YES (8b)|DV/HDR10, PT:LL DA/DTSX, 1TB, UHD-BR
Mini PC: i3/i5-7x00T ([buy](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28hp%2Cdell%2Clenovo%29+%28i3-7100%2Ci5-7400%2Ci5-7500%29&_sacat=179&LH_TitleDesc=0&LH_BIN=1&_sop=15&_udhi=150&_blrs=recall_filtering))|$60|4k@60 (10)|YES (10)|YES (10)|n/ac|1000M|NO|YES (8b)|HDR10, PT:LL DA/DTSX
Mini PC: Intel N95 ([buy](https://www.amazon.com/s?k=n95+n100+mini+pc&crid=GPL0MOIHFBH&sprefix=n95+n100+mini+p%2Caps%2C102&ref=nb_sb_noss_2))|$150|4k@60|YES|YES|ac|1000M|NO|YES (8b)|HDR10, AV1, PT:LL DA/DTSX. w/RAM&SSD
Mini PC: [Intel NUC i3/i5/i7](https://www.intel.com/content/www/us/en/products/boards-kits/nuc.html) ([buy](https://www.newegg.com/p/pl?N=100008345%20601398037%20601398023%20601398021%20601398031%20601407140%20601398048%20601398010%20601398014%20601398049%20601398018%20601398044%20601398008%20601398042%20601398025%20601398029%20601398043%20601398019&Order=1&SrchInDesc=-hunsn%2C-Aittact))|$325-$550|4k@60|YES|YES|ac|1000M|NO|YES (8b)|HDR10, AV1 (3), PT:LL DA/DTSX. add $45 for 8GB RAM/128GB SSD

NOTE: Buy links to Amazon go through Amazon Smile to support your favorite charity

(1) Yes, it will do 4k, but at an abysmal 4k@15Hz

(2) 4k and HDR support using [LibreElec](https://libreelec.tv) >= 10.0.2 and Kodi 

(3) >= 11th gen

(4) Anything other than HEVC is supported at only 1080p

(6) Running Coreelec/Libreelec 

(7) 128GB model 

(8a) FAT32, (8b) FAT32+NTFS 

(9) [Ethernet Adapter](https://www.amazon.com/Cable-Matters-Streaming-Including-Chromecast/dp/B07N2ZHFY9/) for up to 340 Mbps 

(10) w/[CableCreation Active DP 1.4->HDMI Cable](https://www.amazon.com/CableCreation-Unidirectional-DisplayPort-Eyefinity-Multi-Display/dp/B082CXMBCQ) 

## What is the best client device to stream content to my TV?

The Amazon FireTV sticks, Roku and Google ChromeCast w/Google TV products all work very similarly at their respective price levels. Performance, interfaces, remotes all on par with each other with minor differences like types of buttons offered, apps supported, private listening, etc.. Limitations are similar as well; lack of USB storage and no lossless sound output is common across platforms. If you're just looking for something simple to plug into your TV and play Netflix/Hulu/Amazon Prime, $40 or so will get it done.  

Your choice may come down to a particular ecosystem you're already tied to or want to get into.  

If you use/want to use Amazon Alexa a lot you may want to go with a FireTV device.  

If you use/want to use Google Assistant a lot or want an Android TV experience, you may want to go with a Chromecast w/Google TV.  

If you want something more content provider-agnostic that searches across them well and has a lot of curated/free content, you may want to go with a Roku device.  

Once you start looking for advanced features, like external storage, gigabit ethernet, lossless audio or better performance for game streaming/emulation, you should start looking at pricier devices like the Nvidia Shield Pro, Fire TV Cube, and Odroid N2+  


## Can I watch live TV or record it and play it back on my HTPC?

**From an Antenna (OTA) or ClearQAM Cable (unencrypted):** 

Using an over-the-air (OTA) HD antenna avoids the "copy once" problem and most users are surprised by how much mainstream content they can get over the airwaves for free. Alternatively, with Cable, your provider may provide unencrypted ClearQAM channels, usually standard broadcast stations, without a cablecard. Even if you are not a cable TV subscriber, if the cable is connected to the providers network, they may still be sending ClearQAM programming into your home.  

If you use Plex Media Server, you can put a local pcie/usb tuner in your Plex server and set it up for Live TV and DVR, to be accessed by your preferred [Plex client](https://www.plex.tv/media-server-downloads/#plex-app). You can find a list of Plex compatible tuners [here](https://support.plex.tv/articles/225877427-supported-dvr-tuners-and-antennas/).  

If you can't or don't want to place the tuner at your server, you can use a networked tuner like a [HDHomerun](https://www.silicondust.com/) which you can find off ebay for cheap.  

If you don't have ethernet access, you can either use a wifi-capable tuner, like a [Tablo](https://www.tablotv.com) which is simpler to set up, or connect a [HDHomerun](https://www.silicondust.com/) to a [Ethernet->Wifi bridge](https://www.amazon.com/gp/product/B01N5RCZQH).  

For Antennas, stick to well-known brands like Channel Master, Antennas Direct, Winegard and Televés. For reception signal maps check [here](https://www.fcc.gov/media/engineering/dtvmaps), [here](https://www.antennasdirect.com/transmitter-locator.html) and [here](https://rabbitears.info/searchmap.php)  

If you don't want to use Plex to interface with your tuner, but want similar simplicity, you can install the [Channels](https://getchannels.com/) server/dvr somewhere (they support a range of hardware), point it to a networked [HDHomerun](https://www.silicondust.com/) (and ONLY HDHomerun) tuner and then access it with the Channels client app.  

A more involved setup would be connecting a [tuner](https://linuxtv.org/wiki/index.php/ATSC_USB_devices) to a Raspberry PI and using the TVHeadend backend with tvhProxy to get the tuner into Plex. Again, if you don't want to use Plex, skip tvhProxy and simply use Kodi with the TVHeadend client on your frontends to access the TVHeadend backend.  

You can use MCEBuddy to remove commercials and convert your recorded programming to other file formats.  

For a more complete, albeit old, guide to setting up live TV with a generic TV tuner using ServerWMC and MediaBrowser, [see this post.](https://www.reddit.com/r/htpc/comments/2vc16r/guide_network_streaming_of_live_tv_access_tv/). You can use MCEBuddy remove commercials and convert your recorded programming to other file formats for use with PleX Media Server, Kodi or Mediabrowser.  

**From Cable (encrypted):** 

The most common solution is to use a Silicon Dust [HDHomerun Prime](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p4432023.m570.l1313&_nkw=hd+homerun+prime&_sacat=0) tuner, a Cable Card from your cable provider, and Windows Media Center software as the recording front-end. Presently, Windows Media Center is the only known way (using Windows) to record channels marked "copy once" by your cable provider. Different cable providers flag channels differently, and some flag *all* programming this way. Flagged content recorded by WMC can only be streamed to official WMC extenders, which are rare. But you can use ServerWMC to provide live TV to Kodi or MediaBrowser/Emby clients.  
If you only want to watch "copy once" channels, you can use the official HDHR app on Android, Xbox, Windows, etc..  
If you don't need "copy once" channel support, then your options are similar to the Antenna section above, albeit your tuner still being the HDHomerun Prime. That is, adding your tuner into a [Plex Media Server](https://www.plex.tv) or into a [Channels](https://getchannels.com) server and using their respectively client apps, or accessed directly with Kodi/Mediabrowser and its [add-on](https://kodi.wiki/view/Add-on:HDHomeRun).  

**NOTE: Cable Cards are becoming increasingly rare. You should eventually move to streaming from your Cable Service provider or a dedicated TV Streaming Service provider, in the next two options. Also, Windows 10+ will not include or support Windows Media Center or ServerWMC, but it will continue to work with older versions of Windows.**  

**From Cable Service (over the internet):** 

If you don't want to or can't use a tuner with an antenna or cable connection, some TV providers will allow you to pull TV programming over the internet.  

To do this, you need your normal cable subscription service, a login to your provider and a client/server program. The easiest way to currently do this is to install the [Channels DVR Server](https://getchannels.com/dvr-server) software somewhere on your network, configure it to use the [TV Everywhere](https://getchannels.com/tv-everywhere/) feature, with your provider and login credentials and then use the [Channels](https://getchannels.com/apps) client software on your devices to access the channels. On a PC client this can be done either through the server's web ui or via Kodi with the [Channels DVR](https://kodi.wiki/view/Add-on:Channels_DVR) plugin.  

**From Streaming Service (over the internet):** 

Youtube TV, DirectTV Stream, Hulu Live TV or Fubo on the premium end. Philo or Sling TV on the low-end. It depends on the [channels you want](https://www.google.com/search?q=youtube+tv+directv+hulu+fubo+sling+philo&tbs=qdr:m).  


**From your own media content:**

If you want to make virtual TV channels out of your own content, looks at [dizquetv](https://github.com/vexorian/dizquetv) and [ersatztv](https://ersatztv.org) in combination with either a Plex/Jellyfin/Channels DVR-type server or directly with clients like VLC or TiviMate through m3u playlist files.  

## Can I stream/how do I serve my content from another computer or a networked storage device?

Figure out how many clients you will be serving to simultaneously and what types of clients (local or remote). Assume you will be transcoding content for at least 1/3 of the clients (unless you know otherwise). So, for example, if you determine you will have 3 simultaneous clients, assume 1 of them will be transcoding, so choose a server with hardware that can do at least 1 transcode.

Look at the [Sample Builds](/htpc-wiki/sample-builds) page for pre-built and DiY media server solutions based on that. You can buy a very capable media server for under $200. Don't forget to take into account the amount of storage you need, which can be signifigant, whether it be [internal, external, or networked with a NAS](/htpc-wiki/storage). Ripped/Remux 1080p movies can reach 25GB in size EACH, with 4k ones up to 4x that.  

Once you have the hardware you need, connect the media server and/or NAS to your router over ethernet, attach and/or mount the internal/external storage to the server, install and configure media server software, then install the server's player software on your media client devices.  

Media serving software can be PleX Media Server or something similar like Emby/Jellyfin. The advantage of these media servers is that they can transcode the files in real time to meet the needs of your target client device (HTPC, phone, tablet, smart tv, remote client, etc.) and organize your media with metadata. It will serve the media to your client devices or HTPCs using the software's respective client app, over the network. Make sure your network that is serving the clients has bandwidth sufficient to do this. Ideally the clients should be on 100 Mbps ethernet for 1080p content or 1 Gbps ethernet for 4k content. If you're attempting to use wifi instead, make sure the client's bandwidth (via a speed test) is greater than that of your [content's bitrate](https://mediaarea.net/en/MediaInfo).  
  
If you don't want to use media serving softwares, or you don't need real time transcoding, you can simply share your content storage out using a [samba share](https://www.net-usb.com/share-hard-drive-over-network/#usb), whether that be configured in windows or linux, or connected to a router with a USB port. You can then access the network samba share on your media clients, and use normal media players like Kodi, MPC-BE, etc.. to play the content. For those instances where you can't use one of these media players (to access network samba shares), try a DLNA server and client.  



## How do I add Network Attached Storage (NAS) to my network for my HTPC/media devices?

[See our separate wiki page here](/htpc-wiki/storage)  

## What resolution and audio is supported on streaming service X?

The max resolution and audio supported by a particular service on a traditional HTPC varies by the service, OS and program (browser/app) used. For better video, audio and HDR support, use a media device instead.  

The following are the current capabilities of the major streaming services as we know them. These are always subject to change, both for the better and for the worse. If you have any contradicting data, please let us know.  

- [NETFLIX](https://help.netflix.com/en/node/13444?rel=related)  

 *Windows:* (MS Edge/MS Store App) 4k HDR10 DD+ 5.1 Atmos. (Chrome/Firefox) 720p SDR Stereo  

 *Linux:* 720p SDR  

- [AMAZON PRIME VIDEO](https://www.amazon.com/gp/help/customer/display.html/ref=hp_left_v4_sib?ie=UTF8&nodeId=GUVGB3QMQRYRERYW)  

 *Windows:* (MS Edge/Safari) 1080p SDR, (App/Chrome/Firefox) 720p SDR. Stereo  

 *Linux:* 480p SDR, Stereo  

- [HULU](https://help.hulu.com/s/article/video-quality?language=en_US)  

 *Windows:* (MS Store App w/Edge browser as default) 720p SDR, DD+ 5.1. (Browser) 720p SDR, Stereo.   

 *Linux:* 480p SDR, Stereo  
 
- [YOUTUBE](https://support.google.com/youtube/answer/78358?hl=en#:~:text=To%20watch%20YouTube%20videos%2C%20make,Internet%20connection%20with%20500%2B%20Kbps)  

 *Windows:* 4k HDR10, Stereo  

 *Linux:* 4k SDR, Stereo  

- [YOUTUBE TV](https://support.google.com/youtubetv/answer/7129767?hl=en&co=GENIE.Platform%3DDesktop#zippy=%2Cmobile-devices-computers%2Cstreaming-media-players-smart-tvs-game-consoles)  

 *Windows:* 1080p SDR, Stereo  

 *Linux:* 720p SDR, Stereo  

- [HBO NOW/MAX](https://help.hbogo.com/hc/en-us/articles/206950967-What-do-I-need-to-stream-HBO-on-my-computer-)  

 *Windows:* (MS Edge/Safari) 1080p SDR, (Chrome/Firefox) 720p SDR. DD 5.1 (broken)  

 *Linux:* (Chrome/Firefox) 720p SDR?  

- [DISNEY+](https://help.disneyplus.com/csp?id=csp_article_content&sys_kb_id=eac89167db3048900a2af56e0f96193b)  

 *Windows:* (App) 720p SDR DD 5.1. (MS Edge) 720p SDR, (Chrome) 720p SDR, (Firefox) 480p SDR. Stereo.  

 *Linux:* (Chrome/Firefox): 480p SDR, Stereo  

- [APPLE TV+](https://support.apple.com/guide/tvplus/welcome/web)  

 *Windows:* (MS Edge/Chrome/Firefox) 720p SDR?  

 *Linux:* Unknown, but will not be higher than 1080p  

- [TWITCH](https://help.twitch.tv/)  

 *Windows:* 1080p SDR?  

 *Linux:* 1080p SDR?  

- [VUDU](https://support.vudu.com/en_us/categories/general-requirements-r1VPwDURP)  

 *Windows:* (Browser/App) 1080p, Stereo  

 *Linux:* Not supported  

- [PEACOCK TV](https://www.peacocktv.com/help/article/what-devices-and-platforms-are-supported-by-peacock)  

 Windows: (Edge) 1080p? SDR, AAC Stereo  

 Linux: Unknown, but will not be higher than 1080p  

- [PARAMOUNT+](https://help.paramountplus.com/s/article/PD-Supported-Devices)  

 *Windows:* Unknown, but will not be higher than 1080p

 *Linux:* Unknown, but will not be higher than 1080p  

- [DISCOVERY+](https://help.discoveryplus.com/hc/en-us/articles/1500000101182-Browsers-and-devices-supported-by-discovery-)  

 *Windows:* Unknown, but will not be higher than 1080p  

 *Linux:* Unknown, but will not be higher than 1080p  

## How can i rip my DVD/Blu-ray discs and what are some good quality settings to use?

For DVDs and regular HD blu-ray any optical drive that can read the discs will do, internal or external, and you can spend <= $75 on one. For UHD discs, you should have a UHD or UHD-Friendly compatible drive with locked-in firmware. Check our [optical drives section](/htpc-wiki/faq#optical-drives) above.  

You should then use software to rip the content off the disc. It's recommended to do this process in two stages, especially if you need content re-encoded for compatibility or space..  

First, use the [MakeMKV](http://www.makemkv.com/) program to extract the content off the disc. You can choose all the video/audio titles on the disc, just some of them, or just the main one. In the end, this will make a full quality MKV file without changing the format or size of the content. This isn't CPU heavy and can be done on a very minimal system.  

If you're after the best quality, you're done. Play the file with your favorite media player or put the file on your media server storage for serving.  

However, these full quality files are large. DVDs can be up to 9.9GB (11 Mbps), FHD Blu-rays 36GB (40 Mbps), and UHD Blu-Ray 115GB (128 Mbps) for 2 hours worth of content. For this reason, some people move to stage two next and use a program called Handbrake to make the files smaller. It's up to you.  

[Handbrake](https://handbrake.fr/) is used to re-encode content for size, bandwidth and/or compatibility. The goal is to create a file that is highly compatible with client devices and is reasonable on bandwidth use, but doesn't negatively effect the video quality. Re-encoding can take a long time, depending on how fast your CPU is; a modern 4-6 core CPU is ideal, but if you don't care about how long it takes, then it doesn't matter. You can also use a iGPU/dGPU for faster encoding times. Intel QSV (QuickSync) and Nvidia NVENC encoders are supported, but while you reduce encoding times, you also reduce visual quality a bit as GPUs aren't as good as encoding as CPUs.  

In Handbrake..  

On the Summary tab, choose MP4 or MKV for the Format. Neither changes the file size. MP4 is compatible with more devices, but MKV has better embedded subtitle and multi-track audio support. If you're using subtitles and want to embed them into the file, use MKV.  

On the Dimensions tab, if you want to downscale to a different resolution, use Resolution Limit.  

On the Video tab:  

- Video Encoder: h.264 codec, for best client compatibility decoding. Alternatively, the h.265 codec is also possible and will yield better compression on >= 1080p content, but if you have old clients (pre-2016), decoding could be a problem. Consider what client hardware your files will play on first and their capabilities.  

- Framerate : Same as Source, Constant Framerate  

- Encoder Options: Encoder Preset: Medium, Encoder Tune: Film, Encoder Profile: High, Encoder Level: 4.1  

- Quality: Constant Quality is the more efficient encoding method. Use 19 RF (DVD) or 18 RF (Blu-Ray). Use 20 if you're really tight on disk space. If you need to hit a target file size, then use Avg Bitrate instead, but you should use bitrates of >= 1500 kbps (DVD), >= 3000 (720p), >= 7000 (1080p), >= 25000 (4K).  

On the Audio tab, the default is to convert the audio track to a highly compatible AAC, stereo track. If you want to preserve HD audio from your content, you should set the track shown to Passthru instead and then optionally add an additional AAC/Stereo audio track for client compatibility.  

A lot of these settings are subjective, especially video and audio quality. Play around with the settings until you find ones that meet your requirements for a balance between visual/audio quality, disk space and encoding time.  

For a more automated way to do this process, look at [Automatic Ripping Machine](https://github.com/automatic-ripping-machine/automatic-ripping-machine)  


## What do I need for 4k ultraHD compatibility?

**If you want to use a pre-built device/HTPC**

See the top of the [Sample Builds](/htpc-wiki/sample-builds) wiki page or our table of media devices [above](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc).  

**If you're building a traditional DiY HTPC**

*TL;DR*

4k local content: [HDMI 2.0 motherboard](/htpc-wiki/hdmi20) (1.4 if only 30fps non-HDR), >= Intel 7th Gen/Gemini Lake/Athlon 200GE/Ryzen 2200G CPU/GPU **OR** CPU (>= circa 2008) + dGPU >= Nvidia GT1030/AMD RX 550/5x00 **(REC: Ryzen 4600G+B550 mobo)**.  

4k youtube: [HDMI 2.0 motherboard](/htpc-wiki/hdmi20), >= Intel 7th Gen/Gemini Lake/Athlon 200GE/Ryzen 2200G CPU/GPU **OR** CPU (>= circa 2008) + dGPU >= Nvidia GT1030 GDDR5/AMD RX 5x00 **(REC: Ryzen 4600G+B550 mobo)**.  

4k netflix: HDCP 2.2 display, [HDMI 2.0 motherboard](/htpc-wiki/hdmi20), Ryzen 3200G/3400G CPU/GPU **OR** >= Intel 7th Gen/Gemini Lake CPU/GPU **OR** CPU (>= circa 2008) + dGPU >= Nvidia GTX 1050 3GB/AMD RX 550/5x00 **(REC: Ryzen 4600G+B550 mobo)**. Windows 10. Microsoft [HEVC Video Extensions](https://www.microsoft.com/en-us/p/hevc-video-extensions/9nmzlz57r3t7). Intel MEI driver/ME firmware (Intel iGPU). Netflix app/Microsoft Edge browser. Netflix [Premium Plan](https://help.netflix.com/en/node/24926). Netflix [Test Patterns](https://www.netflix.com/title/80018499).  

4k/UHD Blu-Ray disc playing: HDCP 2.2 display, [HDMI 2.0 motherboard w/SGX support](/htpc-wiki/hdmi20), Intel i3/5/7/9 **7th-10th Gen CPU w/iGPU ONLY** **(REC: Intel i3-10100+Gigabyte H370N mobo)**. Windows 10+. Use of a dedicated GPU (dGPU) is **not** supported.  

4k@120Hz: See [Wiki:Video:What options are there for 4k @ 120 Hz video output?](/htpc-wiki/video#what-options-are-there-for-4k--120-hz-video-output)  

MAIN REQUIREMENTS

The major requirements for full 4k compatibility are [HDMI 2.0a](http://www.cnet.com/news/hdmi-2-0-what-you-need-to-know/), [HDCP 2.2](http://www.cnet.com/news/hdcp-2-2-what-you-need-to-know/), hardware HEVC decoding (and support for Intel SGX in the bios if playing UHD blu-ray discs). Anything less will be a limited and incomplete implementation of the upcoming standards.

HARDWARE

Virtually all modern CPUs with integrated graphics can display 4k video. BUT, all of the components in your home theater (TV, AV Receiver and HTPC motherboard) will need to have a HDMI 2.0a or DisplayPort 1.2 port in order to use all sources of 4K content.  
On the AMD side, this starts with the Ryzen 2200G and on with any supported motherboard. Buy a Ryzen 4600G and B550/A520 motherboard and move on.    
On the Intel side, this started with 7th gen Kaby Lake CPUs, but required a [special hdmi 2.0 motherboard](/htpc-wiki/hdmi20); But since 11th gen rocket lake CPUs, any supported motherboard will work. Buy a i3-12100 and H610/B660 motherboard and move on.

If one of the motherboards doesn't fit what you need, or you are upgrading an older, existing system that lacks the above, you can choose a dedicated GPU to add on to your system that has these features. The Nvidia GT 1030 GDDR5 is popular, as is the RX 6400 on the AMD side.

You CAN display 4k video at 30hz via older HDMI 1.4 and 4k video at 60hz via a Displayport 1.2 connection but you will run into other problems. HDMI 1.4 won't support HDCP 2.2/4k blu-ray/Netflix and the Displayport 1.2 connection won't display HDR content, so stick to the more modern iGPUs/dGPUs above.

DRM

If you plan on playing DRM protected content, for instance 4k netflix, you will need to have a HDMI 2.0 port that supports HDCP 2.2 or a Displayport with an active DP 1.x->HDMI 2.0 adapter. This can take the form of at least a Ryzen 3200G/3400G with any supported mobo **OR** Intel 7th-13th Gen/Apollo/Gemini Lake CPU and [supported motherboard](/htpc-wiki/hdmi20) **OR** Any CPU and an add-on dGPU, **only** Nvidia >= GTX 1050 3GB or AMD >= RX 4xx/5xx/5x00/6x00.

More restrictively, if you plan on playing UHD Blu-ray discs, you are further limited to Intel CPUs w/SGX support (Intel i3/5/7/9 7th-10th Gen **ONLY**) + a [HDMI 2.0 motherboard w/SGX support](/htpc-wiki/hdmi20). Dedicated GPUs are **NOT** supported. See [here](https://www.cyberlink.com/support/faq-content.do?id=19144)  

To test for HDCP 2.2 compliance, use [Cyberlink Ultra HD Blu-Ray Advisor](https://www.cyberlink.com/prog/bd-support/diagnosis.do) or [Corel Ultra HD Blu-Ray Check Tool](https://dwnld.windvdpro.com/tools/CorelUltraHDBlurayCheckTool.exe)  

SOFTWARE/CONTENT

The only 4k content supported on a PC are: Local files, UHD blu-ray discs, Youtube and Netflix. See the [section above](/htpc-wiki/faq#what-resolution-is-supported-on-streaming-service-x) on what resolutions are supported for other services. 
If you want access to more 4k content, on your favorite streaming services, use a [media device](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead.  

It is highly likely that the 4K content will be encoded in HEVC (h.265), the successor to the popular and flexible h.264. Hardware decoding of h.265 is limited to:

- Nvidia >= GTX 10xx dGPUs

- Intel 7th-13th Gen/Apollo/Gemini Lake CPU w/iGPU

- AMD >= RX 550/5x00/6x00 dGPUs

- AMD >= Athlon 2x0GE/3000G, >= Ryzen 3 2x00G CPUs. 

All options are sufficient, and have benchmarked playing 4K 400Mbps bitrate videos at >= 70fps ([See Here](https://forum.doom9.org/showthread.php?p=1803012#post1803012)).  Most 24-30fps 4K videos encoded in HEVC have bitrates between 15-60Mbps (Netflix 4K is HEVC encoded at 15Mbps).

HDR is also a popular feature these days. For additional requirements, see the section below.

COST

If you go the CPU w/IGPU route, you can expect to spend about $125 for a CPU (like a Intel i3-12100 or AMD Ryzen 4600g) and between $90-$150 for a Intel B660/AMD B550 motherboard, respectively, depending on the form factor.  

If you go the dedicated GPU route, a Nvidia GT 1030 will cost around $80, while a AMD RX 6400 will cost around $140.  

With either option, expect to spend more than $450 on a complete new build. You can get away with less if you get a used SFF system off ebay and add one of the low profile dedicated GPUs. See the Sample Builds wiki page.  

If you are unsure what to get for your particular requirements, ask us and we will steer you in the right direction.  


## What is HDR video and what do I need to take advantage of it?

HDR stands for High Dynamic Range. It's a technology used to produce better looking video by preserving details in the darkest and lightest portions of a frame resulting in better contrast. Common standards are HDR10, HDR10+ and Dolby Vision.  

For a HTPC, this means HDR support must be in the video, GPU, video interface (HDMI/DP) and ultimately your output device (typically a TV).  

HDR10 is supported on HTPCs under Windows, macOS Catalina, Android and (usually) libreelec/coreelec operating systems. Linux is NOT supported.  

**DOLBY VISION AND HDR10+ MEDIA PROCESSING IS NOT SUPPORTED ON HTPCS**; If you need playback support for these, you'll need a [media device/non-PC](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc), like a Nvidia Shield, Fire TV, Dune HD, etc..  

HDR streaming content is limited thus far and only found on Netflix and Youtube services. If you want access to more HDR content on your favorite streaming services, use a [media device](/htpc-wiki/faq#can-i-use-a-pre-built-media-device-for-my-htpc) instead.  

That being said, HDR is supported on a PC with at least HDMI 2.0a or DisplayPort 1.4 ports. 

If you're not comfortable building DiY, look at the pre-built recommendations at the top of the [Sample Builds](/htpc-wiki/sample-builds) page.  

Otherwise, if you stick to Ryzen APUs or Intel >= 11th gen CPUs below, any paired motherboard will have the HDMI port you need.  

The following CPU iGPUs/APUs are officially supported:  

- Intel 7th-13th (7xxx-13xxx) Gen Core i3/i5/i7/i9, Intel >= 12th gen (G6900/G7400) Celeron/Pentium, Intel N5xxx/N6xxx Jasper Lake (NOT Apollo/Gemini Lake). **(REC: Intel i3-12100+B660 mobo)**  

- AMD >= Ryzen 3 2x00G APU, >= Athlon 2x0GE/3000G **(REC: Ryzen 4600G+B550 mobo)**

It's also available on the following dGPUs: Nvidia GTX >= 950, GT >= 1030, Titan X, Quadro P5000/P6000, AMD RX >= 4x0/5x0/5x00, Radeon 7, Vega 56/64.  

For older DiY motherboard support, reference our [HDMI 2.0 motherboards](/htpc-wiki/hdmi20) page.  

For setting up HDR on your client, [See our separate wiki page here](/htpc-wiki/hdr)  

## Should I buy a low-power version of a CPU?  

*This section applies to DiY*  
CPUs use power, sometimes more than you want. This power usage produces heat, which makes your fans work harder and sound louder to keep the CPU temperature under control. This number is the TDP and is in watts.  
CPU mfgrs like Intel and AMD sometimes make low-power versions of their CPUs with a lower TDP.  
Intel makes 65W and 35W versions of their i3 CPUs, with the 35W version having a "T" suffix (e.g. i3-12100T vs i3-12100) with a signifigantly lower Base Frequency to stay within the 35W limit.  
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
  2. In Windows (AMD): Install the AMD Ryzen Master app. [Lower Base/Boost CPU frequency/TDP or Activate ECO mode](https://www.amd.com/system/files/documents/ryzen-master-quick-reference-guide.pdf).  
  3. In BIOS: Depends on motherboard vendor. Look in the CBS/NBIO/System Config menus to lower the TDP.  
  4. In BIOS: Depends on motherboard vendor. Lower the base/boost cpu frequencies.  
  5. Fan control: Lower the max RPM on your fans causing CPU to throttle its frequencies when hitting thermal limits. Viable, but NOT recommended.  

## How do I set up audio/video on my HTPC?

Audio: [See our separate wiki page here](/htpc-wiki/audio)  

Video: [See our separate wiki page here](/htpc-wiki/video)  


## Do you have any sample builds I can refer to?

[See our separate wiki page here](/htpc-wiki/sample-builds)

