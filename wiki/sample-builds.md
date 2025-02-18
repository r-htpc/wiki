---
description: Information on pre-builts and DiY builds to help you get started with a HTPC, media server, NAS, gaming or specialized setup
keywords: [htpc build, mini pc, pre-builts, media server, emulation, madvr, hdr, all-in-one]
---

# Pre-Built / DiY HTPC Builds

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->
<!-- NA -->

Here you'll find some pre-builts, mini-pcs and sample DiY builds for HTPC, Emulation, Gaming, Media Server, NAS and specialized purposes in their relevant sections. Before going through this page, look at the common scenarios in the [I want a HTPC/media device recommendation, but don't want to get into the complicated details](/wiki/faq#i-want-a-htpcmedia-device-recommendation-but-dont-want-to-get-into-the-complicated-details) section of the FAQ. You may find your specific scenario there and a device to match before you go down this rabbit hole. If what you want is not there, then read on here.  

**There are a lot of options below. You should have a good idea what you're looking for before-hand. Resolution you want to support, video codecs to be decoded, budget, size, used/new, and/or niche capabilities (gaming, 120Hz, output ports). All of these will help you narrow your choice down.**

Keep in mind, the DiY builds are meant as examples for certain usage scenarios, even though they are real builds. You can add/subtract/change certain components to match your specific budget or requirements, but these should be a good starting point. If you're un-sure, check our [Hardware Components Guide](/wiki/components), or post and ask us.  

You can use [PCPartPicker](http://www.pcpartpicker.com/) to help you select parts that will all fit and work together. For current deals/promotions on parts for your build, check [/r/buildapcsales](https://www.reddit.com/r/buildapcsales).  

&nbsp;

<!-- Section -->

## HTPC Pre-builts/Mini-PCs

Pre-builts come in all shapes and sizes. The smallest options are tempting, but usually this means less performance, higher price, and/or more noise. Things like the [SBC](https://en.wikipedia.org/wiki/Single-board_computer) options below will have the highest power efficiency, but also lowest performance, usualy just good enough to get the job done. Intel N/AMD U CPUs (e.g. N150/5560U) have high efficiency. Intel T/AMD GE CPUs (e.g. i3-8100T) medium efficiency. Non-T/non-GE desktop CPUs, low efficiency.  

**Choosing the least expensive option is attractive, but not always the best course of action.** While we recommend some lower-cost chinese vendors below (like Beelink and Minisforum), these may not be for you. With low cost comes limitations like operating system/BIOS support, HDCP, warranty, quality control, security and reliability. If you're not comfortable giving up on those things, spend more to purchase similar speced hardware from other, reputable vendors.  

Some of these are: **Intel (NUC), [Lenovo (ThinkCentre/IdeaCentre)](https://www.lenovo.com/us/en/desktops/subseries-results/?visibleDatas=992%3ASmall%2520Form%2520Factor%2CSmall%2520Form%2520Factor%25C2%25A0), [MSI (DP)](https://www.amazon.com/MSI-12M-407US-Business-i3-12100-Graphics/dp/B0B4BN6TQG?th=1&tag=p00935-20&ascsubtag=02xtx2BszHujAjeR4KoSEAo), Asus (PNxx/PBxx), ASRock (NUC Box, DeskMini/Meet), HP (Prodesk/Elitedesk), Dell (Optiplex), Zotac (ZBOX), Simply Nuc, Shuttle**. We're fond of the Lenovo IdeaCentre Mini and MSI DP series.  

<!-- Sub-Section -->

### 1080p PLAYERS

**TL;DR: If you need extreme power efficiency, then a small ARM-based SBC is ok; but a used Intel 7th gen USFF/SFF/NUC off ebay for $60-100 has better perf / $ and more hw flexibility. For new, an Intel N95 based mini pc <= $150 with mem/storage.**  

 $35-$55: SMALLEST: SBC: (Linux/Coreelec/Libreelec only): [ROCK64-2GB](https://pine64.com/product/rock64-2gb-single-board-computer/) / [Orange Pi 3](https://www.aliexpress.us/item/3256804341645667.html) / [Odroid C4](https://www.hardkernel.com/shop/odroid-c4/). Just good enough, small and cheap.  

 $60-100: SMALL/MEDIUM: Used: HP/Dell/Lenovo - Intel - i3/i5-7100T/7400T/7500T, >= 8GB RAM, >= 120GB disk. [[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28hp%2Cdell%2Clenovo%29+%28i3-7100%2Ci5-7400%2Ci5-7500%29&_sacat=179&LH_TitleDesc=0&LH_BIN=1&_sop=15&_udhi=150&_blrs=recall_filtering)]  

 $80: SMALLER: Used: Intel NUC7i3/NUC7CJYH, >= 8GB, >= 128GB disk. Lower power than HP/Dell/Lenovo above. [[Ebay](https://www.ebay.com/sch/179/i.html?_from=R40&_nkw=nuc+%287100u%2C7260u%2C7300u%2Cj4005%2Cj4025%2Cj5005%29&LH_BIN=1&_sop=15)]  

 $125-160: SMALLER: New: **Intel N95**/N5095 Mini PC ([Minisforum/Beelink/etc..](https://www.amazon.com/s?k=minsforum+beelink+N5095+N95&crid=CZRI7XC6T32)), 8GB RAM, 256GB disk  

 $130-150: SMALLEST: New: Intel N9x/N5105 Nano PC ([GMKTec](https://www.amazon.com/GMKtec-Nucbox5-Desktop-Computer-Windows/dp/B0B75PT2RY)/[Mele](https://www.amazon.com/MeLE-Overclock3C-Windows-Celeron-Computer/dp/B0CB412GMM)), 8GB RAM, 128GB-256GB disk  

<!-- Sub-Section -->

### 4K HDR PLAYERS

**TL;DR: A [Beelink EQR6](https://www.amazon.com/Beelink-Windows-Celeron-Graphics-Computer/dp/B08QCMSR6R) or better ($270+) is ideal. If you're on a budget, then an Intel [N150](https://www.amazon.com/s?k=intel+n150+pc&rh=n%3A13896591011&ref=nb_sb_noss) for the bare minimum ($150)**  
**If you're looking for 4K Netflix/HDCP support, look at [name brand options](/wiki/sample-builds#specialized-4k-netflix)**

$70-$85: SMALLEST: SBC: w/CoreELEC OS, 32GB MicroSD, AC Adapter 

 - *Used for:* H264/H265, VP9 **local** content, Kodi-based interface, ext. storage, lowest power 
   - [Odroid C4](https://www.hardkernel.com/shop/odroid-c4/) ($60) 
   - **[Odroid N2+](https://www.hardkernel.com/shop/odroid-n2-with-2gbyte-ram-2/) ($72)** 

$150-$400: SMALLER: Intel/AMD Mini PC, 8GB+ RAM, 256GB+ SSD

- *Used for:* H264/H265, VP9, **AV1** local content, 4k YT, 4k Netflix **([name brand options](/wiki/sample-builds#specialized-4k-netflix))**, web browsing, **int. 2.5" storage**, plex server (G3/Cubi), light gaming (EQR/SER), lower power.  
  - **Intel: [GMKtec G3 Plus](https://www.amazon.com/GMKtec-G3-Plus-Upgraded-Computer/dp/B0DM25BD7Y) (N150) ($150+)**
  - **AMD: [Beelink EQR6](https://www.amazon.com/Beelink-Windows-Celeron-Graphics-Computer/dp/B08QCMSR6R) (6600H) ($270)**
  - Intel: MSI Cubi [NUC B](https://www.amazon.com/MSI-Cubi-Business-Processor-Ethernet/dp/B0CD96ZWL8?th=1) ($250) / [NUC 1M](https://www.newegg.com/msi-cubi-nuc-1m-011bus-intel-core-3-100u/p/N82E16856167202?Item=N82E16856167202) ($380+[RAM](https://pcpartpicker.com/products/memory/#xcx=0&Z=8192001,16384001,16384002,32768002&ff=ddr5_sodimm&sort=price)+[SSD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&t=0&D=1&A=240000000000,512000000000&sort=price&page=1))
  - AMD: [Beelink EQR6](https://www.amazon.com/s?k=eqr6+6900hx&i=electronics&crid=39BXXMKRACXZJ&sprefix=eqr6+6900hx%2Celectronics%2C140&ref=nb_sb_noss_2) (6900HX) ($350)  
<!--  - Intel: [Beelink SEI 11/12](https://www.amazon.com/s?k=sei11%7Csei12%7C11320h%7C1235u%7C12450h&rh=n%3A13896591011&ref=nb_sb_noss) ($320) -->

$100-$500: SMALL/MEDIUM: Intel - i3/i5-7xxx+ 8GB (2x4GB) RAM, 256GB ssd/1TB hdd: 

 - *Used for:* H264/H265, VP9, **AV1 (Optiplex [3-7]000/Lenovo/MSI)** local content, 4k Netflix/YT, web browsing, **int. 3.5" storage/ODD (SFF/MT models)**, plex server, low power (xxxxT cpu models).  
   - USED: [Dell Optiplex xx50-xx90](https://www.ebay.com/sch/i.html?_fsrp=1&_from=R40&_nkw=%28optiplex%29+%283050%2C3060%2C3070%2C3080%2C5060%2C5070%2C5080%2C7060%2C7070%2C7080%29+%28i3-8100%2Ci3-9100%2Ci3-10100%2Ci5-7400%2Ci5-7500%2C7600%2Ci5-8400%2C8500%2Ci5-8600%2Ci5-9400%2C9500%2C9600%29&_sacat=0&LH_TitleDesc=0&_sop=15&_oaa=1&_dcat=179&rt=nc&LH_BIN=1) + [HDMI 2.0 card](https://www.ebay.com/sch/i.html?_from=R40&_nkw=dell+hdmi+2.0+%28HXPK2%2C1KNYY%2CR07CP%2C5N1NY%29&_sacat=0&_sop=12) / [3000-7000](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%28optiplex+3000%29+%28i3%2Ci5%2Ci7%29&_sacat=171957&_odkw=%28optiplex%29+%283000%29+%28i3%2Ci5%2Ci7%29&_osacat=171957&LH_BIN=1&_sop=15&LH_PrefLoc=2) + [HDMI 2.0 card](https://www.dell.com/en-us/shop/dell-daughterboard-i-o-hdmi-card/apd/3v9n2/controller-cards) ($100-$300)
   - **NEW: [Lenovo IdeaCentre Mini](https://www.lenovo.com/us/en/p/desktops/ideacentre/500-series/ideacentre-mini-gen-8-(1l-intel)/90w2000gut) / [Lenovo Neo 50s Gen 4 SFF](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=lenovo+neo+50s&_sacat=179&LH_TitleDesc=0&_odkw=neo+50s&_osacat=179&_sop=15&LH_ItemCondition=3) / [MSI PRO DP21 iX](https://www.amazon.com/s?k=msi+dp21&i=electronics&s=price-asc-rank) ($400-600)** 

$150-$500: SMALL/MEDIUM: AMD - Ryzen 3x00G-5x00G, 8GB (2x4GB) RAM, 256GB ssd/1TB hdd

 - *Used for:* H264/H265, VP9 local content, 4k Netflix/YT, web browsing, **int. 3.5" storage/ODD (SFF/MT models)**, **light gaming**, low power (xxxxGE cpu models).  
   - USED: [HP EliteDesk 705 G5](https://www.ebay.com/sch/179/i.html?_from=R40&_nkw=hp+705+g5+%283200g%2C3400g%29&LH_TitleDesc=1&_sop=15&LH_PrefLoc=2&rt=nc&LH_BIN=1) + [HDMI 2.0 card - 3TK75AA](https://www.ebay.com/sch/i.html?_from=R40&_nkw=hdmi+705+%283TK75AA%2CL25757%29&_sacat=0&_odkw=hdmi+%283TK75AA%2CL25757%29&_osacat=0&_nls=2&_dmd=1) ($140-$300)
   - NEW: [MSI DP20](https://www.ebay.com/sch/179/i.html?_from=R40&_nkw=msi+dp20&_sop=15&LH_BIN=1&rt=nc&LH_ItemCondition=1000%7C1500) / [Lenovo M75s Gen 2 SFF](https://www.ebay.com/sch/i.html?_from=R40&_nkw=lenovo+m75s+gen+2&_sacat=179&LH_TitleDesc=0&_sop=15&rt=nc&LH_ItemCondition=1500%7C1000) + [CableCreation Active DP 1.4->HDMI Cable](https://www.amazon.com/CableCreation-Unidirectional-DisplayPort-Eyefinity-Multi-Display/dp/B082CXMBCQ) ($300-$600)

<!-- Sub-Section -->

### Specialized: Emulation/Light Gaming/Game Streaming

- Game Streaming:
  - <= 4K@60Hz: GMKTec G3 Plus (N150)
  - 4K@120Hz: See "Specialized: 4K@120Hz" section
- Emulation/Light Gaming:
  - $85-100: Low (<= Gamecube/PS1)
    - [Odroid N2+](https://www.hardkernel.com/shop/odroid-n2-with-4gbyte-ram-2/) (S922X) (Fanless)
    - [Intel NUC 8i3/8i5](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=nuc+%288i3%2C8i5%2C8109u%2C8130u%2C8th%2C8259u%29&_sacat=179&LH_TitleDesc=1&_odkw=nuc+%288i3%2C8i5%2C8109u%2C8130u%2C8th%29&_osacat=179&_sop=15&LH_PrefLoc=2) (USED)
  - $150-200: Med (<= Wii/PS2)
    - [Odroid H4](https://www.hardkernel.com/shop/odroid-h4/) (N97) (Fanless)
    - [HP EliteDesk 705 G5](https://www.ebay.com/sch/179/i.html?_from=R40&_nkw=hp+705+g5+%283200g%2C3400g%29&LH_TitleDesc=1&_sop=15&LH_PrefLoc=2&rt=nc&LH_BIN=1) (AMD 3400G)
    - [Minisforum UN300](https://www.amazon.com/MINISFORUM-LPDDR5-i3-N300-Threads-USB3-2/dp/B0CQYW121V) (N300)  
  - $300: Med+ (<= Switch)
    - [Beelink SER5](https://www.amazon.com/s?k=beelink+5800h&crid=3AUBU1SOXW7YK&sprefix=beelink+5800h%2Caps%2C163&ref=nb_sb_noss_1) (AMD 5800H)  
  - $350-400: High (<= PS3)
    - [Beelink EQR6](https://www.amazon.com/s?k=eqr6+6900hx&i=electronics&crid=39BXXMKRACXZJ&sprefix=eqr6+6900hx%2Celectronics%2C140&ref=nb_sb_noss_2)/[Minisforum UM690S](https://www.amazon.com/MINISFORUM-UM690-6900HX-Threads-Bluetooth5-2/dp/B0BP1S1YNS/) (6900HX)  
  - $500+: Ultra (<= Xbox 360)
    - [Beelink SER7](https://www.amazon.com/Beelink-SER7-7840HS-Computer-Display/dp/B0CQT9N951)/[Minisforum UM790 Pro](https://store.minisforum.com/collections/game-mini-pc/products/minisforum-um790-pro?variant=44134865731829) 

 See [ETA PRIME](https://www.youtube.com/@ETAPRIME) YT channel for Emulation device reviews  

<!-- Sub-Section -->

### Specialized: 4K Netflix

Intel 7th gen+ or AMD 3200+ G/U/H/HX APUs + HDCP 2.2+ implemented on HDMI 2.0 port + Windows 10+  

- Dell Optiplex/HP Prodesk/Elitedesk + HDMI 2.0 card (see recs in 4K HDR players above)
- ASRock [NUC/4x4 Box](https://www.newegg.com/ASRock-Industrial-Mini-PC-Barebone/BrandSubCat/ID-223387-309?Order=1), [DeskMini/DeskMeet](https://www.newegg.com/ASRock-Mini-PC-Barebone/BrandSubCat/ID-1944-309)
- [Lenovo Ideacentre/Neo/M75](https://www.lenovo.com/us/en/c/desktops/thinkcentre/?sortBy=priceUp&visibleDatas=699%3AWindows%252011%2520Pro%252064%2CWindows%252011%2520Home%252064%2CWindows%252010%2520Pro%252064) (see recs in 4K HDR players above)
- [MSI Cubi/Pro DP series](https://www.amazon.com/s?keywords=Mini+Computers&i=computers&rh=n%3A13896591011%2Cp_123%3A378555&dc&c=ts&qid=1733595152&rnid=85457740011&ts_id=13896591011&ref=sr_nr_p_123_10&ds=v1%3AnQRfur4qf8GhElQv2EyLSUgtMG4sr3SJOY94hUGfkfE) (see recs in 4K HDR players above)
- Intel/Asus NUC 7+ (i3-i9)
- [Asus ExpertCenter PN42+](https://www.amazon.com/s?k=asus+expertcenter&i=computers&rh=n%3A13896591011&s=price-asc-rank)

<!-- Sub-Section -->

### Specialized: 4K@120Hz

- **[UM760 Slim](https://store.minisforum.com/products/minisforum-um760-slim)**, [SER6 Max](https://www.google.com/search?q=ser6+max&oq=ser6+max), [Gigabyte Brix Extreme](https://www.newegg.com/p/pl?d=gigabyte+brix+extreme), [Venus UM790](https://store.minisforum.com/collections/amd-%C2%AE-ryzen-%C2%AE/products/minisforum-um790-pro), [ASRock 4x4 7535U/8640U](https://www.newegg.com/p/pl?N=50223387&d=4x4&Order=1), [Intel NUC 12/13](https://www.newegg.com/p/pl?N=100008345%2050001157%20601331497&Order=1&SrchInDesc=nuc+12) + [Cable Matters Thunderbolt->HDMI 2.1 Cable](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08QDV5H4M) + Display w/HDMI DSC support
- [What options are there for 4k @ 120 Hz video output?](/wiki/video#what-options-are-there-for-4k--120-hz-video-output)  

<!-- Sub-Section -->

### Specialized: Dolby Vision / HDR10+

- *Local:* Ugoos AM6B Plus/Dune HD Box R Plus (8K: Ugoos AM8 Pro) + CoreElec. *Local+Streaming:* Nvidia Shield Pro (DV), FireTV Cube (HDR10+/DV)
- **No passthrough on a traditional/DiY HTPC**  

<!-- Sub-Section -->

### Specialized: 3D MVC/Frame-Packed

- [HTPC w/Windows or Mac](https://www.reddit.com/r/htpc/comments/115ap94/how_to_get_full_hd_3d_frame_packing_from_a_pc_or/), Odroid N2+ + CoreElec, Vero V / Ugoos AM6B Plus / Zidoo Z9X w/Kodi-based player

<!-- Sub-Section -->

### Specialized: Fanless

- [Odroid H4](https://www.hardkernel.com/shop/odroid-h4/), [Asus PN42](https://www.asus.com/us/displays-desktops/mini-pcs/pn-series/asus-expertcenter-pn42/), [Zotac CI6xx](https://www.zotac.com/us/product/mini_pcs/all?field_filter_m_series_tid%5B%5D=2229&field_filter_m_processor_tid%5B%5D=2241&field_filter_m_processor_tid%5B%5D=2242&field_filter_m_processor_tid%5B%5D=2243&field_filter_m_processor_tid%5B%5D=2510), [Asus PL64](https://www.asus.com/displays-desktops/mini-pcs/pl-series/mini-pc-pl64/), [Mele Quieter](https://www.amazon.com/s?k=mele+quieter&i=electronics), Intel/Asus NUC+[Akasa Case](https://www.akasa.co.uk/update.php?tpl=list%2FCHASSIS+POWER.tpl&type=CHASSIS+POWER&type_sub=FANLESS+CASES&fval=all), [SimplyNUC PorCoolPine](https://simplynuc.com/embedded-industrial/), [OnLogic NUCs](https://www.onlogic.com/computers/nuc/)  

<!-- Sub-Section -->

### Specialized: Optical/Toslink output

- [NUC11PHKi7C](https://www.intel.com/content/dam/www/public/us/en/documents/product-briefs/nuc-11-enthusiast-product-brief.pdf), [NUC7PJYH](https://www.google.com/search?q=NUC7PJYH&oq=NUC7PJYH)
- Anything + [Cubilux USB -> TOSLINK](https://www.amazon.com/Cubilux-TOSLINK-Converter-Compatible-Computer/dp/B0B2DBGKL3) 

<!-- Sub-Section -->

### Specialized: HDMI-CEC

- [RPI4](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) / [ROCK64-2GB](https://pine64.com/product/rock64-2gb-single-board-computer/) (full)
- [Intel branded NUCs](https://www.intel.com/content/www/us/en/support/articles/000023500/intel-nuc/intel-nuc-kits.html) (just power states, or full with [pulse8 adapter](https://www.pulse-eight.com/c/59)), MSI Cubi NUC 1M
- [Asus PN41](https://www.asus.com/us/displays-desktops/mini-pcs/pn-series/mini-pc-pn41/) / PN42 / [PN50](https://www.asus.com/us/displays-desktops/mini-pcs/pn-series/mini-pc-pn50/) / PN51 / PN64 / [PL64](https://www.asus.com/displays-desktops/mini-pcs/pl-series/mini-pc-pl64/) (just wake state)  

<!-- Sub-Section -->

### Specialized: Media Server w/Transcoding

- Light: GMKtec G3 Plus, [Pre-built NAS](/wiki/storage#pre-built-nas) - ~3x 4k transcodes
- Medium: Beelink SEI 12 i5-12450H, [Media Server Builds](/wiki/sample-builds#nasmedia-server-builds) - ~6x 4k transcodes
- Heavy: Minisforum NAB6 Lite, [Intel NUC 11/12/13 i5](https://www.newegg.com/p/pl?N=100008345%2050001157%20601398044%20601412542%20601398019%20601412544%20601398041%20601412545%20601398018&Order=1) - ~12x 4k transcodes.
<!-- - [DiY NAS/Media Server Build w/i5-12500+](https://r-htpc.github.io/wiki/sample-builds#nasmedia-server-builds) - ~18 4k transcodes -->

<!-- Sub-Section -->

### Specialized: Media client, server, storage system combos

- $350 - 1080p, low-medium 4k content, Light Transcoding: Fire TV 4k (client) + GMKtec G3 Plus (server) + Terramaster F2-212 (storage)

  - 4k HDR10/DV-5/8, Dolby TrueHD Atmos, DTS, 3x4k,10x1080p transcodes, 2xHDDs (WD Ultrastar/Seagate Exos), Ubuntu/Windows, Plex Pass/Jellyfin

- $600 - 4k, high-bitrate, Light Transcoding: Nvidia Shield Pro (client) + GMKtec G3 Plus (server) + Terramaster F4-212 (storage)

  - 4k HDR10/DV-5/7/8, Dolby TrueHD Atmos, DTS:X, 3x4k,10x1080p transcodes, 4xHDDs (WD Ultrastar/Seagate Exos), Ubuntu/Windows, Plex Pass/Jellyfin

- $750 - 4k, high-bitrate, Medium Transcoding: Nvidia Shield Pro (client) + Beelink SEI 12 i5-12450H (server) + Terramaster F4-212 (storage)

  - 4k HDR10/DV-5/7/8, Dolby TrueHD Atmos, DTS:X, 6x4k,20x1080p transcodes, 4xHDDs (WD Ultrastar/Seagate Exos), Ubuntu, Plex Pass/Jellyfin
  - For more transcodes, switch server to [Minisforum NAB6 Lite](https://store.minisforum.com/products/minisforum-nab6?variant=45797300863221)

<!-- Section -->

## HTPC DIY builds

<!-- Sub-Section -->

### 4K HDR PLAYER (2L)

TL;DR: You want a small 4K@60 HDR player and don't need any, or need only minimal 2.5" local storage.  

Tiny, simple player. Good for 4K playback; local content, netflix, youtube, HDR, browsing, and game streaming; light 1080p gaming.  

If you want **AV1** decoding to future-proof, go with the alternative Ryzen 8500G with respective changes (DeskMini X600, DDR5) parts or an Intel i3-12100 with respective HW changes (DeskMini B760/B660, etc..). You will give up gaming performance with the Intel version.

If you can't find the DeskMini case and still want to build, look at the Inwin Chopin alternate build. There's also a stack of good Tiny cases in the [Cases section](/wiki/faq#cases) of the Wiki FAQ. You should use [Pico PSU 150W+](https://www.mini-box.com/Power-Supplies-Kits)-style kits for these.  

If you can't afford the optional CPU cooler, pop the top off the stock AMD one to make it fit.  

You could add some media storage with a [2.5" HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&f=3&sort=ppgb&A=1900000000000,20000000000000&page=1), but these cases are NOT for internal 3.5" HDD media storage - they're too small for that.  If you want to stay within this size case, either use external USB HDDs or buy/build a [NAS](/wiki/storage#pre-built-nas-list) for backend storage. Otherwise, look at the all-in-one builds below.  

<!-- Sub-Section -->

**Deskmini - MOBO built-in, PSU external, 1.9L** 

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE/PSU		|Asrock Deskmini X300W					|$170	|Amazon	|MOBO/PSU inc - 6.1"x6.1"x3.1" ALT: [X600](https://www.newegg.com/asrock-deskmini-x600-amd-ryzen-8000-7000-series/p/N82E16856158096) ($180)
CPU			|AMD Ryzen 5500GT APU (65W)					|	$110	|[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)	|ALT: [Ryzen 8500G](https://pcpartpicker.com/product/y3XV3C/amd-ryzen-5-8500g-41-ghz-6-core-processor-100-100000931box) ($150)
MEM			|Crucial 2x8GB DDR4-3200 SODIMM - CT2K8G4SFRA32A	|$40		|[amazon](https://www.amazon.com/Crucial-2x8GB-Laptop-Memory-CT2K8G4SFRA32A/dp/B08C4WV6FT)	|ALT: [Crucial 2x8GB DDR5-5600 SODIMM](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr5&ff=ddr5_sodimm&Z=16384002&sort=price&page=1) ($50)
STORAGE	 	|WD SN580 500GB NVMe M.2 SSD	(OS)				|$40		|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|ALT: WD Black SN770 1TB M.2 ($70)
COOL	 	|Noctua NH-L9a-AM4 CPU Cooler, 37mm					|$45		|[pcpartpicker](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=14000000,47000000&c=33&W=0&sort=price&page=1)	|OPTIONAL. Quieter than stock cooler
TOTAL		|											|$405	||

**Inwin Chopin - MOBO separate, PSU internal, 3.3L** 

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE/PSU	|Inwin Chopin/BQ656					|	$100		|[google](https://www.google.com/search?q=inwin+bq656+chopin&udm=28)	|PSU included - 8.6" x 9.6" x 3.3"
MOBO		|Gigabyte A520I AC ITX					|	$110	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&f=8&s=33&sort=price&page=1)			|ALT: [ASRock A620I Lightning](https://pcpartpicker.com/products/motherboard/#f=8&sort=price&xcx=0&s=41) ($120)
CPU			|AMD Ryzen 5500GT APU (65W)					|	$110	|[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)	|ALT: [Ryzen 8500G](https://pcpartpicker.com/product/y3XV3C/amd-ryzen-5-8500g-41-ghz-6-core-processor-100-100000931box) ($150)
MEM			|TEAMGROUP T-Force Vulcan Z 2x8GB DDR4-3200			|	$35		|[pcpartpicker](https://pcpartpicker.com/products/memory/#Z=16384002&sort=price&xcx=0&ff=ddr4&S=3200,7200&L=160,180)	|ALT: [Crucial 2x8GB DDR5-5600](https://pcpartpicker.com/product/y4BzK8/crucial-classic-16-gb-2-x-8-gb-ddr5-5600-cl46-memory-ct2k8g56c46u5) ($45)
STORAGE	 	|WD SN580 500GB NVMe M.2 SSD	(OS)				|$40		|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|ALT: WD Black SN770 1TB M.2 ($70)
COOL		|Thermalright AXP90-X47 CPU Cooler, 47mm			|	$30		|[pcpartpicker](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=14000000,47000000&c=33&W=0&sort=price&page=1)	|OPTIONAL: Quieter than stock cooler.
TOTAL		|										|	$425	|	|

<!-- Sub-Section -->

### 4K HDR ALL-IN-ONE PLAYER (9L)

TL;DR: You want a 4K@60 HDR player, may want 3.5" HDD media storage and want a value build that doesn't break the bank.  

This build is good for 4K playback; local content, netflix, youtube, HDR, and game streaming. Light 720p/1080p gaming can also be had on it. 

If you want **AV1** decoding to future-proof, go with the alternative Ryzen 8500G with respective changes (DeskMeet X600, DDR5) parts or an Intel i3-12100 with respective HW changes (DeskMeet B760/B660, etc..). You will give up gaming performance with the Intel version.

Expect HDR processing and upscaling with madVR to operate at a basic level - don't expect to be doing heavy upscaling here without a dGPU.  

You can add 2x3.5" HDD content storage for an all-in-one. Since optional, it's not included in the price.  

Choose the DeskMeet option if you don't have a height restriction (like a small media cabinet) or want a full-height ITX dGPU, otherwise choose the Apex build or the slimmer variation with or without LP dGPU. If height restriction and full-height dGPU needed, look at the [ML07](https://www.silverstonetek.com/en/product/info/computer-chassis/ML07/). 

*Larger Slimmer variation*: 12-16L, 4" (H): Change CASE to [InWin BL040](https://www.amazon.com/InWin-BL040-mATX-Desktop-Black/dp/B0964K2W4R) (PSU still included) ($100) or a Silverstone [ML03](https://pcpartpicker.com/product/bWR48d/silverstone-case-ml03b)/[ML04](https://pcpartpicker.com/product/fsw323/silverstone-case-ml04b) (add an [ATX PSU](https://pcpartpicker.com/products/power-supply/#sort=price&e=4,3,2,1&th=1&m=8,337,50,11,14,106,101,18,229,51,71,63,441,113,56)). You can change to a [uATX mobo](https://pcpartpicker.com/products/motherboard/#xcx=0&f=7&c=145&sort=price&page=1) with these cases, which is cheaper than ITX. LP dGPU and 3xHDDs possible

*Larger Cube variation*: 12-16L: $50 more. Change CASE to [Silverstone SG13B](https://www.amazon.com/SilverStone-Technology-Mini-ITX-Computer-SST-SG13B-USA/dp/B07MNC3JCB) (1xHDD) or [Jonsbo C6 mATX](https://pcpartpicker.com/product/WMCZxr/jonsbo-c6-microatx-mini-tower-case-c6-black) (1-2xHDD), add an [ATX PSU](https://pcpartpicker.com/products/power-supply/#sort=price&e=4,3,2,1&p=1,2&th=1). ITX+ dGPU possible

**DeskMeet - Cube, 8.8L** 

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE/MOBO/PSU		|[Asrock DeskMeet X300W w/500W PSU](https://www.asrock.com/nettop/AMD/DeskMeet%20X300%20Series/index.asp#Specification)					|$190	|[newegg](https://www.newegg.com/asrock-deskmeet-x300w-b-bb-box-us/p/N82E16856158083)	|6.6" (W) x 9.3" (D) x 8.7" (H). ALT: [X600](https://www.newegg.com/asrock-deskmeet-x600w-deskmeet-x600-series/p/N82E16856158094) ($200)
CPU				|Ryzen 5500GT (65W)							|$110	|[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)	|ALT: [Ryzen 8500G](https://pcpartpicker.com/product/y3XV3C/amd-ryzen-5-8500g-41-ghz-6-core-processor-100-100000931box) ($150)
MEM			|TEAMGROUP T-Force Vulcan Z 2x8GB DDR4-3200			|	$35		|[pcpartpicker](https://pcpartpicker.com/products/memory/#Z=16384002&sort=price&xcx=0&ff=ddr4&S=3200,7200&L=160,180)	|ALT: [Crucial 2x8GB DDR5-5600](https://pcpartpicker.com/product/y4BzK8/crucial-classic-16-gb-2-x-8-gb-ddr5-5600-cl46-memory-ct2k8g56c46u5) ($45)
STORAGE			|WD SN580 500GB NVMe M.2 SSD TLC				|$40	|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|
STORAGE			|4TB 7200rpm 3.5" HDD			|$40	|[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/4TB?order=onlinecustomerprice:asc&show=48)	|OPTIONAL. ALT: [6TB ($70), 8TB ($90)](https://serverpartdeals.com/collections/manufacturer-recertified-drives?pf_t_interface_type=interface%3ASATA&pf_t_capacity=capacity%3A6TB&pf_t_capacity=capacity%3A8TB)
COOL		|Thermalright AXP90-X47 CPU Cooler, 47mm			|	$30		|[pcpartpicker](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=14000000,47000000&c=33&W=0&sort=price&page=1)	|OPTIONAL: Quieter than stock cooler
TOTAL			|											|$375	|	|

**Apex - Slim, 9.6L** 

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE/PSU			|[Apex MI-008 Mini ITX w/250W PSU](https://www.apextechusa.com/products.asp?pID=171)					|$70	|[pcpartpicker](https://pcpartpicker.com/product/hHg323/apex-case-mi008)	|8.7" (W) x 13.5" (D) x 5.1" (H).
CPU				|Ryzen 5500GT (65W)							|$110	|[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)	|ALT: [Intel i3-12100](https://pcpartpicker.com/product/qrhFf7/intel-core-i3-12100-33-ghz-quad-core-processor-bx8071512100)
MOBO			|ASRock B550M-ITX/ac					|$130	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&f=8&s=33&sort=price&page=1)	|ALT: INTEL: [ASRock B760M-ITX/D4](https://pcpartpicker.com/product/3xLFf7/asrock-b760m-itxd4-wifi-mini-itx-lga1700-motherboard-b760m-itxd4-wifi)
MEM			|TEAMGROUP T-Force Vulcan Z 2x8GB DDR4-3200			|	$35		|[pcpartpicker](https://pcpartpicker.com/products/memory/#Z=16384002&sort=price&xcx=0&ff=ddr4&S=3200,7200&L=160,180)	|
STORAGE			|WD SN580 500GB NVMe M.2 SSD TLC				|$40	|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|
STORAGE			|4TB 7200rpm 3.5" HDD			|$40	|[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/4TB?order=onlinecustomerprice:asc&show=48)	|OPTIONAL. ALT: [6TB ($70), 8TB ($90)](https://serverpartdeals.com/collections/manufacturer-recertified-drives?pf_t_interface_type=interface%3ASATA&pf_t_capacity=capacity%3A6TB&pf_t_capacity=capacity%3A8TB)
COOL			|Thermalright AXP90-X36 CPU Cooler, 36mm					|$25	|[pcpartpicker](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=14000000,47000000&c=33&W=0&sort=price&page=1)	|
TOTAL			|											|$410	|	|

<!-- Sub-Section -->

<!-- Commented out since AV1 wordage added to builds above 

### 4K HDR AV1 ALL-IN-ONE PLAYER (12L)

HTPC that can hardware decode the next-gen AV1 codec without buying a dGPU, which costs as much as this whole system. Also can do 4K local/youtube/netflix HDR as well as fit a couple 3.5" HDDs.

MicroATX is the cheapest, but ITX alternatives aren't much more.

*Tiny variation*: 1.9L: Change CASE & MOBO to a ASRock Deskmini B660W ($180) (mobo included), change MEM to [SO-DIMM](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr4&ff=ddr4_sodimm&sort=price&S=2666,8000&Z=16384002)s. No 3.5" HDD content storage possible because of size, only [2.5" HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&f=3&sort=ppgb&A=1900000000000,20000000000000&page=1).  

*Larger Slim variation*: 16L: Change CASE to Silverstone [ML03](https://pcpartpicker.com/product/bWR48d/silverstone-case-ml03b)/[ML04](https://pcpartpicker.com/product/fsw323/silverstone-case-ml04b). Add an [ATX PSU](https://pcpartpicker.com/products/power-supply/#sort=price&e=4,3,2,1&p=1,2&th=1).  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE	|InWin Slim MicroATX BL040 Case w/300W PSU			|	$100		|	[amazon](https://www.amazon.com/InWin-BL040-mATX-Desktop-Black/dp/B0964K2W4R)			|	ALT: ITX: Apex MI-008 Mini ITX w/250W PSU (9.6L) ($60)
MOBO	|MSI PRO B760M-P DDR4 MicroATX					|	$100		|	[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&s=40&f=7&sort=price&page=1)		|	ALT: ITX: [pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&sort=price&f=8&s=40)
CPU		|Intel i3-12100 - 60W							|	$120		|	[pcpartpicker](https://pcpartpicker.com/product/qrhFf7/intel-core-i3-12100-33-ghz-quad-core-processor-bx8071512100)		| ALT: Intel G7400 ($80)
MEM		|Teamforce Vulcan Z DDR4-3200 2x8GB				|	$35		|	[pcpartpicker](https://pcpartpicker.com/product/2Bnypg/team-t-force-vulcan-z-16-gb-2-x-8-gb-ddr4-3200-cl16-memory-tlzgd416g3200hc16fdc01)	|	ALT: [pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&sort=price&S=3000,8000&Z=16384002)
STORAGE		|Teamgroup MP33 512GB NVMe M.2 SSD 			|	$40		|[pcpartpicker](https://pcpartpicker.com/product/Brvqqs/team-mp33-512-gb-m2-2280-nvme-solid-state-drive-tm8fp6512g0c101)	|ALT: WD Black SN770 500 GB M.2 ($40)
TOTAL							|			|	$395		|			|

-->

<!-- Sub-Section -->

### FANLESS 4K HDR PLAYER (4.6L)

Completely fanless solution for 4k HDR media playback and/or 720p/1080p gaming emulation.  

You could add some media storage with [2.5" HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&f=3&sort=ppgb&A=1900000000000,20000000000000&page=1)s, but this is not for internal 3.5" HDD media storage - 
it's too small for that. Look at the [HD Plex H3 (11L)](https://hdplex.com/hdplex-h3-v3-fanless-computer-chassis.html) or [FC8 Alpha](https://www.quietpcusa.com/Streacom-HTPC-Cases/Streacom-FC8-ALPHA-HTPC-Chassis) chassis or the next super low power build instead.  
These cases are popular and low production, so don't be surprised if they're out of stock.  

If you can afford it, get the HD Plex 250W GaN ATX PSU, else the DC-ATX Pico versions are fine for APU-only builds.  

A comparable, similarly priced alternative is the [Streacom FC8 Alpha](https://www.quietpcusa.com/Streacom-HTPC-Cases/Streacom-FC8-ALPHA-HTPC-Chassis). The [DB1](https://www.quietpcusa.com/streacom-htpc-cases/streacom-1-fanless-chassis) is also an option and much cheaper than the others, though will limit you to 45W ECO mode on the CPU.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE	|	HD Plex H1 v3				|	$215	|	[HD Plex](https://hdplex.com/hdplex-h1-v3-fanless-computer-case.html)	|	no psu inc., 10.6" x 10.4" x 2.5"
CPU	|	Ryzen 5500GT APU (65W)				|	$110	|	[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)		|	ALT: [Intel i3-12100](https://pcpartpicker.com/product/qrhFf7/intel-core-i3-12100-33-ghz-quad-core-processor-bx8071512100)
MOBO	|	ASRock B550M-ITX/ac	|	$130	|	[pcpartpicker](https://pcpartpicker.com/products/motherboard/#f=8&s=33&sort=price&page=1)	|	ALT: [ASRock B760M-ITX/D4](https://pcpartpicker.com/product/3xLFf7/asrock-b760m-itxd4-wifi-mini-itx-lga1700-motherboard-b760m-itxd4-wifi)
MEM	|	Teamgroup Vulcan Z DDR4-3200 2x8GB		|	$35	|	[pcpartpicker](https://pcpartpicker.com/product/2Bnypg/team-t-force-vulcan-z-16-gb-2-x-8-gb-ddr4-3200-cl16-memory-tlzgd416g3200hc16fdc01)		|	ALT: [pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&sort=price&S=3000,8000&Z=16384002)
STORAGE	|	WD Black SN770 500 GB NVMe M.2 SSD	|	$45	|	[pcpartpicker](https://pcpartpicker.com/product/nWC48d/western-digital-500-gb-m2-2280-nvme-solid-state-drive-wds500g3x0e)		|	ALT: WD SN580 1TB
PSU	|	HD Plex 200W (DC-ATX)		|	$80	|	[HD Plex](https://hdplex.com/hdplex-200w-dc-atx-power-supply-12v-48v-wide-range-voltage-input.html)			|	ALT: [HDPlex 250W GaN ATX](https://hdplex.com/hdplex-fanless-250w-gan-aio-atx-psu.html) / [picoPSU-160-XT 160W (DC-ATX-2)](https://www.mini-box.com/picoPSU-160-XT)
PSU	|	Dell 230W+ 19.5V 7.4x5.0mm Adapter (for DC-ATX)		|	$30	|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=dell+19.5V+adapter+230+240+330&_sacat=0&_odkw=dell+230w&_osacat=0)	|	ALT: [192W AC adapter](https://www.mini-box.com/12v-16A-AC-DC-Power-Adapter) (for DC-ATX-2)
TOTAL|						|	$645	|	|	|	

<!-- Sub-Section -->

### Super low power all-in-one fanless player (3.3L)

Low power, fanless CPU (6W), 4k@60Hz playback, 4k netflix/YT, HDR. Case specced can fit 1x3.5" HDD. This is for someone who wants a low power build with the flexibility to choose ram/ssd/HDD/PCIe vs a pre-built mini PC which does not afford that flexibility or expansion.  
For 2x3.5" HDDs, use a Apex MI-008 case (you will not use the PSU) and a SATA power splitter.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE|Goodisory A01/MX01 ITX|$45|[amazon](https://www.amazon.com/Goodisory-Aluminum-Mini-ITX-Computer-Tempered/dp/B07GYP2TWC)|7.9" x 7.9" x 3.3" ALT: Apex MI-008/ML03
CPU/MOBO|ASRock N100DC-ITX, 6W|$130|[newegg](https://www.newegg.com/p/N82E16813162133)|[specs](https://www.asrock.com/mb/Intel/N100DC-ITX/).
MEM|G.Skill Ripjaws V 1x16GB DDR4-3200 DIMM|$35|[pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr4&ff=ddr4&sort=price&S=3200,8000&Z=8192001,16384001)|ALT: 1x8GB ($20)
STORAGE			|WD SN580 250GB NVMe M.2 SSD TLC				|$30	|[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#t=0&A=250000000000,22000000000000&f=122080&D=1&sort=price&page=1)	|
STORAGE			|4TB 7200rpm 3.5" HDD			|$40	|[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/4TB?order=onlinecustomerprice:asc&show=48)	|OPTIONAL. ALT: [6TB ($70), 8TB ($90)](https://serverpartdeals.com/collections/manufacturer-recertified-drives?pf_t_interface_type=interface%3ASATA&pf_t_capacity=capacity%3A6TB&pf_t_capacity=capacity%3A8TB)
POWER			|19V 65W AC-DC Adapter|$25	|[amazon](https://www.amazon.com/Pwr-Power-Supply-Intel-FSP065-10AABA/dp/B076L52WV4)	|
TOTAL||$265||

<!-- Sub-Section -->

### MadVR upscaling all-in-one player (14L)

This is a build with a dGPU for MadVR upscaling/tonemapping that's going to provide better visual quality than the iGPU on a CPU. Other features include 4k@60 playback, 4k netflix/YT, HDR, and medium 1080p gaming.

The Nvidia GTX 1660 chosen is the most powerful, reasonably-priced, GPU you will find. If you need something new, then the RTX 3050 6GB.  

We don't go beyond a mid-level GPU here for MadVR because we feel you start to get into diminishing returns on visual quality, while incurring more power usage and heat.  

You can alternately change the CASE to a Silverstone [GD09 (26.8L)](https://www.silverstonetek.com/en/product/info/computer-chassis/GD09/) w/a ATX PSU, to get more room for storage, better cpu and/or a bigger, quieter cooler. For a low profile dGPU, look at the ML09 (7L)/ML03 (15.7L)

If you can't afford to do a new build or only need reasonable upscaling, you can buy a [2nd-hand SFF pre-built](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=sff+%28i5-7400%2Ci5-7500%2Ci5-7600%2Ci5-8400%2Ci5-8500%2Ci5-8600%29+-optiplex+-prodesk&_sacat=0&LH_TitleDesc=0&_fsrp=1&_odkw=sff+%28i5-7400%2Ci5-7500%2Ci5-7600%29+-optiplex+-prodesk&_osacat=0&_sop=15) off ebay and pop a GTX 1050 Ti low profile in it.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE|Silverstone ML07|$105|[amazon](https://www.amazon.com/SilverStone-Technology-Mini-ITX-Computer-ML07B/dp/B00K8CIZYS?th=1)|[specs](https://www.silverstonetek.com/en/product/info/computer-chassis/ML07/). ALT: Silverstone [GD09](https://www.silverstonetek.com/en/product/info/computer-chassis/GD09/)
CPU|Intel i5-12400F, 65W|$115|[pcpartpicker](https://pcpartpicker.com/product/pQNxFT/intel-core-i5-12400f-25-ghz-6-core-processor-bx8071512400f)|ALT: Intel i5-12100F
MOBO|ASRock B760M-ITX/D4|$150|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&f=8&s=40&sort=price&page=1)|ALT: GD09: [MSI PRO B660M-A DDR4 MicroATX](https://pcpartpicker.com/product/KKbTwP/msi-pro-b660m-a-ddr4-micro-atx-lga1700-motherboard-pro-b660m-a-ddr4) ($120)
MEM|Corsair Vengeance LPX 16GB 2x8GB DDR4-3200|$40|[pcpartpicker](https://pcpartpicker.com/product/p6RFf7/corsair-memory-cmk16gx4m2b3200c16)|
GPU|Nvidia GTX 1660 6GB|$100|[ebay](https://www.ebay.com/sch/27386/i.html?_fsrp=1&rt=nc&_from=R40&LH_TitleDesc=0&LH_PrefLoc=2&_nkw=gtx+1660&LH_BIN=1&_sacat=27386&_sop=15&_oac=1&LH_ItemCondition=1500%7C1000%7C2500%7C3000)|<= 330 mm. ALT: [Nvidia RTX 3050 6GB](https://pcpartpicker.com/products/video-card/#xcx=0&c=572,518&sort=price&page=1) ($170)
STORAGE			|WD SN580 500GB NVMe M.2 SSD TLC				|$40	|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|OS/App Drive
STORAGE			|4TB 7200rpm 3.5" HDD			|$40	|[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/4TB?order=onlinecustomerprice:asc&show=48)	|OPTIONAL. ALT: [6TB ($70), 8TB ($90)](https://serverpartdeals.com/collections/manufacturer-recertified-drives?pf_t_interface_type=interface%3ASATA&pf_t_capacity=capacity%3A6TB&pf_t_capacity=capacity%3A8TB)
COOL	|	Thermalright AXP120-X67	CPU Cooler	|	$35	|[pcpartpicker](https://pcpartpicker.com/product/K2cG3C/thermalright-axp120-x67-59-cfm-cpu-cooler-axp120-x67)	|OPTIONAL. ALT: GD09: Thermalright Silver Soul 135 ($40)
PSU|Silverstone SX500-G 500W SFX|$110|[pcpartpicker](https://pcpartpicker.com/products/power-supply/#xcx=0&th=5&sort=price&m=8,337,50,11,14,101,17,18,27,28,94,29,229,51,71,63,441,56&A=450000000000,2050000000000)|ALT: GD09: [500W+ ATX](https://pcpartpicker.com/products/power-supply/#xcx=0&th=1&sort=price&m=8,337,50,11,14,17,18,27,28,94,29,229,51,71,63,441,56&e=4,2)
TOTAL||$660||

<!-- Sub-Section -->

### UHD MakeMKV Ripping/Handbrake Transcoding Machine (16-32L)

A build for ripping DVD/FHD Blu Ray and UHD Blu Ray discs. As such, it has space for 5.25 drives and 5-6 HDDs to make this into a NAS/media server as well.  
If you don't need the drive space and want something smaller, consider the Silverstone ML03/ML04 (16L) or In Win CE685 (12L).   
Alternatively, if you want a different form factor or more HDD space look at Silverstone's GD06 (4)/TJ08B-E (6)/GD07 (8)/GD08 (9).  

This uses a modern 10-core CPU w/IGPU for very fast Handbrake transcoding performance. This is a high watt part and necessitates a good tower CPU cooler. If you go with one of the smaller/shorter cases, you can either lower the TDP on the CPU or switch to a i5-12400 w/stock cooler.  

Standard software for ripping is: [MakeMKV](https://www.makemkv.com) to rip a disc to a full quality file, and then [Handbrake](https://handbrake.fr) to optionally transcode it down for size and client compatibility. Check the [ripping section](/wiki/faq#how-can-i-rip-my-dvdblu-ray-discs-and-what-are-some-good-quality-settings-to-use) of our FAQ page for detailed instructions. Check the flashing guide on the [makemkv forum](https://forum.makemkv.com/forum/viewforum.php?f=16) for drive firmware, if you intend to do UHD ripping.   
For automated ripping on disc insert, look at [Automatic Ripping Machine](https://github.com/automatic-ripping-machine/automatic-ripping-machine) (ARM), which is a front-end to makemkv/handbrake. Its setup on Linux is not for the faint of heart. 
Alternatively, on Windows look at [Staxrip](https://github.com/staxrip/staxrip) or the old [Autorip](https://videoscripts.wordpress.com/2011/11/16/autorip-updated-3/).  

If you can't afford to spend this much, buy a 2nd-hand pre-built and make some upgrades. Look at the "Medium NAS / Media Server (9-26L)" build below; they come with DVD drives standard. You can then upgrade to FHD/UHD ripping with a [LG BU40N](https://www.ebay.com/itm/332968508515?epid=21020020503&hash=item4d86783c63:g:DpkAAOSwF7lcHJ6b) FHD/UHD blu-ray drive, a [Slimline SATA Adapter](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=slimline+sata+to+sata+adapter+-usb+-nvme+-mount&_sacat=0&LH_TitleDesc=0&_odkw=slimline+sata+to+sata+adapter+-usb+-nvme&_osacat=0), and be out for $250.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE	|Silverstone PS07				|$110	|	[pcpartpicker](https://pcpartpicker.com/product/qmtCmG/silverstone-case-sstps07b)	| [specs](https://www.silverstonetek.com/en/product/info/computer-chassis/PS07/). ALT: Silverstone ML03
CPU		|Intel i5-12600K CPU, 125W				|$175	|	[pcpartpicker](https://pcpartpicker.com/product/BB4Ycf/intel-core-i5-12600k-37-ghz-6-core-processor-bx8071512600k)	|	ALT: i5-12400 ($135)
MOBO	|ASRock B760M Pro RS	|$125	|	[pcpartpicker](https://pcpartpicker.com/product/pTbTwP/asrock-b760m-pro-rs-micro-atx-lga1700-motherboard-b760m-pro-rs)	|	ALT: [Other uATX mobos](https://pcpartpicker.com/products/motherboard/#xcx=0&c=154,163,152,162&f=7&sort=price&mt=ddr5)
MEM		|Teamgroup T-Create Expert 32GB 2x16GB DDR5-6000			|$85	|	[pcpartpicker](https://pcpartpicker.com/product/H9CZxr/teamgroup-t-create-expert-32-gb-2-x-16-gb-ddr5-6000-cl30-memory-ctced532g6000hc30dc01)	|	ALT: Teamgroup Elite 16GB 2x8GB DDR5-5200 ($45)
STORAGE	|LG WH16NS40 UHD Blu-Ray Drive			|$70	|	[pcpartpicker](https://pcpartpicker.com/product/QZ6BD3/lg-optical-drive-wh16ns40)	|	ALT: ASUS BW-16D1HT ($100)
STORAGE	|WD SN770 1TB NVMe M.2 SSD		|$70	|	[pcpartpicker](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e)	|	ALT:  Teamgroup Cardea Zero Z440 1TB
COOL	|Thermalright Peerless Assassin CPU Cooler				|$40	|	[pcpartpicker](https://pcpartpicker.com/product/hYxRsY/thermalright-peerless-assassin-120-se-6617-cfm-cpu-cooler-pa120-se-d3)	|	ALT: Thermalright AXP120-X67 ($40)
PSU		|Corsair RM650 Full Modular ATX PSU		|$80	|	[pcpartpicker](https://pcpartpicker.com/products/power-supply/#xcx=0&th=1&sort=price&m=8,337,50,11,14,17,18,27,28,94,29,229,51,71,63,441,56&e=4,2)	|	ALT: Silverstone Essential 750W ($75)
SOFTWARE	|MakeMKV Beta/Full		|FREE/$60	|	[makemkv](https://www.makemkv.com/buy/)	|Free with beta license key posted each month
TOTAL	|										|$755	|					|

<!-- Sub-Section -->

### CHEAPEST 4K HDR/ALL-IN-ONE PLAYER - NEW (12L)

TL;DR: You want 4K@60 local/youtube/netflix HDR on a real PC, may want HDD media storage and want the cheapest build with new hardware that we're comfortable recommending.  

Not the prettiest case, but slim and gets the job done at 12 liters.  

Light 720p gaming can be had here, if you need.  

You can add one or more 3.5" HDD content storage for an all-in-one.  

*Tiny variation*: 1.9L: $25 more. Change CASE & MOBO to a ASRock Deskmini X300W ($180) (mobo included), change MEM to [SO-DIMM](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr4&ff=ddr4_sodimm&sort=price&Z=8192001,8192002)s. No 3.5" HDD content storage possible because of size, only [2.5" HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&f=3&sort=ppgb&A=1900000000000,20000000000000&page=1).  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE	|InWin Slim MicroATX BL040 Case w/300W PSU		|$100	|[amazon](https://www.amazon.com/InWin-BL040-mATX-Desktop-Black/dp/B0964K2W4R)	|13" x 14.4" x 3.8"
MOBO	|ASRock B450M-HDV R4.0 MicroATX				|$60  	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&s=33&sort=price&f=7)	| 
CPU	|AMD Ryzen 3200G (65W)				|$80	|[pcpartpicker](https://pcpartpicker.com/product/J8drxr/amd-ryzen-3-3200g-36-ghz-quad-core-processor-yd3200c5fhbox)	|ALT: Ryzen 5500GT ($110) 
MEM	|G.Skill Value DDR4-2400 2x4GB		|$25  	|[pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&sort=price&Z=8192002,16384002&ff=ddr4)	|
STORAGE	|Patriot P300 256GB M.2 SSD (OS/APPS)				|$20	|[pcpartpicker](https://pcpartpicker.com/product/rWxbt6/patriot-p300-256-gb-m2-2280-nvme-solid-state-drive-p300p256gm28)	|
STORAGE			|4TB 7200rpm 3.5" HDD			|$40	|[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/4TB?order=onlinecustomerprice:asc&show=48)	|OPTIONAL. ALT: [6TB ($70), 8TB ($90)](https://serverpartdeals.com/collections/manufacturer-recertified-drives?pf_t_interface_type=interface%3ASATA&pf_t_capacity=capacity%3A6TB&pf_t_capacity=capacity%3A8TB)
TOTAL	|							|$285  	|	|

<!-- Sub-Section -->

### CHEAPEST 4K HTPC PLAYER - USED

TL;DR: Cheapest hardware for 4k@60Hz, HDR and/or 4k netflix player, or a dead simple media server.  

For the insanely frugal, the absolute cheapest way to buy/build a PC for use as a 4k@60Hz player - using used hardware off eBay.  

We will use a i5-4570 CPU and Nvidia GT 1030 GDDR5 GPU (not DDR4).

If you have more specific GPU usage needs, then..  
4K local+youtube: The quoted config  
4K local+netflix: [AMD RX 550 4GB](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=rx+550+%22hdmi%22&_sacat=27386&LH_TitleDesc=0&_fsrp=1&_odkw=rx+550+4GB+%22hdmi%22&_osacat=27386&LH_BIN=1&_sop=15&LH_PrefLoc=2&_udhi=120.00) ($50)  
4K local+netflix+youtube: [Nvidia GTX 1050 Ti 4GB](https://www.ebay.com/sch/27386/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=gtx+1050+ti&LH_BIN=1&_sacat=27386&LH_TitleDesc=0&_sop=15&_udhi=120.00&LH_ItemCondition=1000%7C2500%7C3000%7C1500) ($70) + Mini Tower case or low-profile card for $20 more.  
1080p: no dGPU  

The quoted config here is with a SFF form factor case, for use with a low-profile GPU, but if you want one of the Mini Tower form factor versions shown as ALT: below , that's fine as well.  

If you don't even need 4k or are using it as a dead simple media server, drop the GPU and you have yourself a very capable all in one 1080p box for $50. Getting one with an included SSD for your OS drive will be very helpful for responsiveness on these low-end machines.  

[Sample i3/i5 Ebay Search](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-4570%2Ci5-4590%2Ci7-4770%29+%28sff%2Cmt%2Cdt%29&_sacat=179&LH_TitleDesc=0&_blrs=recall_filtering&_osacat=179&LH_BIN=1&_sop=15&_geositeid=0&_udhi=120.00)  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE			|HP Prodesk 400/600/800 G1, Dell Optiplex 3020/9020/XE2, Lenovo M73/M83/M93p, HP Z230	|$50	|[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-4570%2Ci5-4590%2Ci7-4770%29+%28sff%2Cmt%2Cdt%29&_sacat=179&LH_TitleDesc=0&_blrs=recall_filtering&_osacat=179&LH_BIN=1&_sop=15&_geositeid=0&_udhi=120.00)	|ALT: Mini Tower: Dell 3020/7020/9020/3647 MT, HP 600/800 G1 MT, Lenovo M73, HP PRO Z230
CPU/MEM			|Intel i5-4570 w/4-8GB DDR3 RAM - Included in above		|NA		|Ebay	|CPU Passmark: 5000-7000
STORAGE			|250GB-500GB HDD/SSD - Included in above									|NA		|Ebay	|ALT: 128GB 2.5" SSD ($15)
GPU				|Nvidia GT 1030 GDDR5											|$50	|[Ebay](https://www.ebay.com/sch/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=GT+1030+gddr5&_sacat=27386&LH_BIN=1&LH_TitleDesc=0&_sop=15&_udhi=120.00&LH_ItemCondition=1000%7C1500%7C2500%7C3000)	|ALT: RX 550 4GB Low Profile ($50)
TOTAL			|																		|$100	|		|

<!-- Section -->

## NAS/Media Server builds

There are many tiers of builds depending on what tasks you want to accomplish, how much internal capacity you need and your budget level. We'll provide a couple common builds here in increasing complexity. There is no one-size-fits-all and the options can be wide and varied.  

<!-- Sub-Section -->

### $100 Small Media Server (1.2L) - Used

This is a good setup to get your feet wet in media serving in a very small package. A used pre-built is cheaper and easier to get going if you're new to this. If you're not comfortable buying used, [this](https://www.amazon.com/GMKtec-G3-Plus-Upgraded-Computer/dp/B0DM25BD7Y) is comparable.  

Most people will use it with Plex Media Server to serve media up to clients, but you can serve media up to Kodi clients over a network/samba share just as well.  

If you're using it with Plex, it will [Direct Play](https://support.plex.tv/articles/200430303-streaming-overview/) content to multiple clients just fine (even 4k). If you need to transcode content either internally or remotely, it 
will [transcode](https://support.plex.tv/articles/200430303-streaming-overview/) 2x 1080p streams or 4x 720p streams using software/cpu transcoding in the free version of Plex Media Server.  

If you need to transcode more streams than this (either because your internal clients don't support your media's codecs and/or because you have a lot of remote users), pay for a [Plex Pass](https://www.plex.tv/plex-pass/) (or use Jellyfin) and it will then [hw transcode](https://support.plex.tv/articles/115002178853-using-hardware-accelerated-streaming/) more 1080p and 4k HEVC/H264 streams.  

It's preferred to use an SSD for your OS drive and for storing Plex Metadata. Purchase one separately as per the parts list below or get one included.

With a form factor this small, you should use USB external drives, in the short-term, like a [WD Elements/Easystore](https://www.bestbuy.com/site/wd-easystore-8tb-external-usb-3-0-hard-drive-black/6425302.p?skuId=6425302&utm_source=feed), for media storage. It is possible to use an internal [2.5" HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=900000000000,22000000000000&sort=price&f=3&t=5000,5200,5400,5640,5700,5760,5900,5940,7200&page=1) up to 5TB if you use an M.2 SSD for your OS. If you want more reliable, long-term storage, look at the next build w/internal 3.5" HDD(s) instead or a NAS from our [Storage Setup Guide](/wiki/storage).  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|HP/Dell/Lenovo Micro PC	|	$80	|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400t%2Ci5-8500t%29&_sacat=179&_fsrp=1&_odkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400t%2Ci5-8500t%2Ci5-7400t%2Ci5-7500t%29&_osacat=179&LH_BIN=1&_sop=15&LH_PrefLoc=2&_udhi=150)	|	Prodesk G4, Optiplex 3060/5060/7060, Thinkcentre M720q/M920q
CPU/GPU		|Intel i5-8500T	|	Included|	NA|		35W, 6C/6T. ALT: [i5-7500T](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-7400t%2Ci5-7500t%29&_sacat=179&_fsrp=1&_odkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400t%2Ci5-8500t%29&_osacat=179&LH_BIN=1&_sop=15&LH_PrefLoc=2&_udhi=150) ($-15)
MEM			|8 GB+ DDR4|	Included|	NA|		NA
STORAGE		|256GB M.2 SSD (OS/APPS)		|	$25|	[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=240000000000,22000000000000&t=0&sort=price&f=122030,122042,122060,122080)|		OPTIONAL, If not included in ebay build.
STORAGE		|WD 8-20TB USB HDD (MEDIA)		|$160-350		|	[Best Buy](https://www.bestbuy.com/site/wd-easystore-8tb-external-usb-3-0-hard-drive-black/6425302.p?skuId=6425302&utm_source=feed)		| OPTIONAL, if not included in ebay build or don't have. ALT: [2.5" SATA HDD](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=900000000000,22000000000000&sort=price&f=3&t=5000,5200,5400,5640,5700,5760,5900,5940,7200&page=1)
OS			|Ubuntu 24/Windows 1x Pro				|$0			|	[Ubuntu](https://ubuntu.com/download)	|	
SOFTWARE	|Plex Media Server						|$0			|	[Plex](https://www.plex.tv/downloads)	|	Free
LICENSE		|Plex Pass								|$120		|	[Plex](https://www.plex.tv/plex-pass/)	|	OPTIONAL. Lifetime cost or $40/year, $5/month.	
TOTAL		|				|	$105	||

<!-- Sub-Section -->

### $135 Medium NAS / Media Server (9-26L) - Used

This is also a good setup to get your feet wet. A used pre-built is cheaper and easier to get going if you're new to this. A NAS/media server with these specs has the potential to handle anything you can throw at it with the ability to have some internal media storage. If you're not comfortable buying used, [these](https://www.ebay.com/sch/i.html?_fsrp=1&_from=R40&LH_TitleDesc=1&LH_PrefLoc=2&LH_ItemCondition=1000&Form%2520Factor=Mini%2520Tower%7CSmall%2520Form%2520Factor%2520%2528SFF%2529%7CTower%7CMini%2520Pc&_nkw=%28hp%2Cdell%29+%28i3%2Ci5%2Ci7%29&_sacat=179&LH_BIN=1&_sop=15&rt=nc&Processor=Intel%2520Core%2520i7%252012th%2520Gen%252E%7CIntel%2520Core%2520i5%252013th%2520Gen%252E%7CIntel%2520Core%2520i5%252011th%2520Gen%252E%7CIntel%2520Core%2520i3%252012th%2520Gen%252E%7CIntel%2520Core%2520i5%25209th%2520Gen%252E%7CIntel%2520Core%2520i7%25209th%2520Gen%252E%7CIntel%2520Core%2520i3%252011th%2520Gen%252E%7CIntel%2520Core%2520i7%252010th%2520Gen%252E%7CIntel%2520Core%2520i5%252012th%2520Gen%252E%7CIntel%2520Core%2520i3%25209th%2520Gen%252E%7CIntel%2520Core%2520i3%252010th%2520Gen%252E%7CIntel%2520Core%2520i5%252010th%2520Gen%252E%7CIntel%2520Core%2520i7%252013th%2520Gen%252E%7CIntel%2520Core%2520i7%252011th%2520Gen%252E&_oaa=1&_dcat=179) are comparable.  

Most people will use it with Plex Media Server to serve media up to clients, but you can serve media up to Kodi clients over a network/samba share just as well.  

If you're using it with Plex, it will [Direct Play](https://support.plex.tv/articles/200430303-streaming-overview/) content to multiple clients just fine. If you need to transcode content either internally or remotely, it 
will [transcode](https://support.plex.tv/articles/200430303-streaming-overview/) 2x 1080p streams or 5x 720p streams using software/cpu transcoding in the free version of Plex Media Server.  

If you need to transcode more streams than this (either because your internal clients don't support your media's codecs and/or because you have a lot of remote users), pay for a Plex Pass (or use Jellyfin) and it will then [hw transcode](https://support.plex.tv/articles/115002178853-using-hardware-accelerated-streaming/) 4x 4k streams or 15x 1080p HEVC/H264 streams using the iGPU.  

Internally this server will support 1x M.2 NVME SSD drive, 1x 2.5" SSD/HDD and 1x 3.5" HDD.  
If you want to fit more than 1x 3.5" HDDs internally, look at these versions:  
2x HDDs: [Lenovo M710T](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=lenovo+%28m710t%2C720t%29+%287100%2C7400%2C7500%2C7700%2C8400%2C8500%2C8700%29&_sacat=179&LH_TitleDesc=0&_odkw=lenovo+%28m710t%2C720t%29+%287400%2C7500%2C7700%2C8400%2C8500%2C8700%29&_osacat=179&LH_BIN=1&_sop=15&_udhi=200) (15.5L), [HP 800 G4 SFF](https://www.ebay.com/sch/i.html?_from=R40&_nkw=hp+800+g4+sff+%287500%2C7600%2C7700%2C8400%2C8500%2C8600%2C8700%29&_sacat=179&LH_BIN=1&_sop=15) (10.4L), [Lenovo P320 SFF](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=lenovo+p320+%287500%2C7600%2C7700%29+-tiny+-micro+-mini&_sacat=0&_odkw=lenovo+p320+%28i5%2Ci7%29+-tiny+-micro+-mini+8500&_osacat=0&LH_BIN=1&_sop=15) (12.9L)  
3x HDDs: [HP 800 G3/G4 TWR](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=HP+%28600%2C800%29+%28G3%2CG4%29+%28twr%29+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29&_sacat=179&_odkw=HP+Prodesk+%28600%2C800%29+%28G3%2CG4%29+%28twr%29+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29&_osacat=179&_sop=15) (20.8L), [Lenovo P330 MT](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=lenovo+p330+%28i3%2Ci5%2Ci7%29+-sff&_sacat=179&_odkw=lenovo+p330+%28i3%2Ci5%2Ci7%29&LH_BIN=1&_osacat=179&_sop=15) (20.3L)  
4x HDDs: [Dell Precision 3620](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=dell+3620+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29&_sacat=179&LH_TitleDesc=0&_odkw=dell+t3630+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29&_osacat=179&_sop=15&LH_PrefLoc=2) (27.4L), [HP Z2 G4 Tower](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%22HP+Z2%22+G4+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29+-SFF+-mini+-small&_sacat=179&LH_TitleDesc=0&_odkw=%22HP+Z2%22+G4+%287100%2C7400%2C7500%2C7700%2C8100%2C8400%2C8500%2C8700%29+-SFF&_osacat=179&_sop=15&LH_PrefLoc=2) (26.1L), [Lenovo P320 Tower](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=lenovo+p320+%287500%2C7600%2C7700%29+-tiny+-micro+-mini&_sacat=0&_odkw=lenovo+p320+%28i5%2Ci7%29+-tiny+-micro+-mini+8500&_osacat=0&LH_BIN=1&_sop=15) (25L)  

It's preferred to use an SSD for your OS drive and for storing Plex Metadata. You can either buy the system with an SSD included, or buy it bare, purchasing one separately as per the parts list below. The latter is preferrable as you have more control over size/brand/form factor.  

For media content storage, either use the HDD (if provided in the one you buy), or replace it with a bigger one. You can get an 8TB drive for about $100. Check our [Storage Setup Guide](/wiki/storage#hard-drives) drive list for more options. If you want to throw a bunch of drives at it, either go with one of the bigger cases above or add a Terramaster [F4-212 NAS](/wiki/storage#pre-built-nas-list). If you want to go beyond this you'll want to build everything internally with the next NAS/Media Server build below as a starting point.  

A good serving solution with the below system would be a M.2 SSD for OS/apps, a large 3.5" internal HDD, Ubuntu 24, docker and the plex docker container.

Windows would be fine for ease of administration, but you should go with Ubuntu, OpenMediaVault or Unraid on the Linux-side for more advanced usage, like Docker, and/or have better multi-disk volume management.  

See our [Storage Setup Guide](/wiki/storage) for more information on software, drives, and pre-built NASes.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
PC			|Lenovo M720s SFF PC					|$100		|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28m720s%29+%288400%2C8500%2C8600%2C8700%29&_sacat=171957&_odkw=%28m710s%2Cm720s%29+%288400%2C8500%2C8600%2C8700%29&_osacat=171957&_sop=15&LH_PrefLoc=2&_udhi=250) | 8.4L, [specs](https://psref.lenovo.com/syspool/Sys/PDF/ThinkCentre/ThinkCentre_M720_SFF/ThinkCentre_M720_SFF_Spec.PDF). ALT: [HP/Dell](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28hp%2Cdell%29+SFF&_sacat=179&_fsrp=1&_odkw=%28i5-8400%2Ci5-8500%2Ci5-8600%2Ci7-8700%29+%28hp%2Cdell%29+%28-micro%2C-DM%2C-MFF%29+%28-8400T%2C-8500T%29&_osacat=179&LH_BIN=1&_sop=15&LH_PrefLoc=2&_udhi=250)
CPU/GPU			|Intel i5-8400							|Included	|	NA			|	65 W, 6C/6T. ALT: [i5-7400](https://www.ebay.com/sch/i.html?_from=R40&_nkw=m710s%20%287400%2C7500%2C7600%2C7700%29&_sacat=171957&LH_TitleDesc=0&_sop=15&LH_PrefLoc=2&rt=nc&_udhi=250) (-$10)
MEM/STORAGE	|8GB RAM, HDD/SSD/Bare					|Included	|	NA			|	
STORAGE		|500GB M.2 NVMe SSD (OS/APPS)		|$35		|	[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=480000000000,22000000000000&t=0&sort=price&f=122030,122042,122060,122080&D=1)		| OPTIONAL, if not included in ebay build.
STORAGE		|WD 8-20 TB 3.5" SATA HDD (MEDIA)		|$100-350		|	[Serverpartdeals](https://serverpartdeals.com/collections/wd-ultrastar-sata-hard-drives?sort=price-ascending&pf_t_condition=condition%3AManufacturer+Recertified&pf_t_condition=condition%3ANew)		| OPTIONAL, if not included in ebay build or don't have.
OS			|Ubuntu 24/Windows 1x Pro				|$0			|	[Ubuntu](https://ubuntu.com/download)	|	
SOFTWARE	|Plex Media Server						|$0			|	[Plex](https://www.plex.tv/downloads)	|	Free
LICENSE		|Plex Pass								|$120		|	[Plex](https://www.plex.tv/plex-pass/)	|	OPTIONAL. Lifetime cost or $40/year, $5/month.	
TOTAL		|										|$135		|	NA			|

<!-- Sub-Section -->

### $650 Medium NAS / Media Server (19.5L) - New

This build can be seen as a culmination of the previous two builds, a media server and a NAS combined, while using new hardware.  

The Node 304 is tailor made for this kind of NAS and the Intel CPU will give you hardware media transcoding and video out for administration and even all-in-one use, if you really wanted.  

Nothing else here is too surprising. High value ram and ssd perform well and don't break the bank.  

This is configured below with 24TB of usable space with protection (12TBx3 = 36TB - 12TB parity drive = 24TB), but you can pack it all the way up to 110TB usable with protection (6x22TB-22TB parity). We use highly reliable, well-priced Exos/Ultrastar HDDs here.   

If you want to bulk up past 6 drives, look at the Coolermaster N400 or Node 804 case for up to 10 drives, with the uATX motherboard and the optional 9207-8i HBA in the parts list.  

If used as a Plex server, you can [Direct Play](https://support.plex.tv/articles/200430303-streaming-overview/) a couple dozen stream and [transcode](https://support.plex.tv/articles/200430303-streaming-overview/) 6 concurrent 1080p streams with software transcoding. If you need more transcodes than that, do [hardware igpu transcoding](https://support.plex.tv/articles/115002178853-using-hardware-accelerated-streaming/) with a purchased Plex Pass and a linux docker/VM in Unraid. That'll get you 6x4k/20x1080p AV1/HEVC/H264 transcodes. Alternatively, if you didn't want to buy a Plex Pass, use JellyFin; or use an i5-12400 to get software transcoding for 9x1080p/1x4k 50Mbps streams and upgrade to a Plex Pass later. 

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE|Fractal Design Node 304|$100|[newegg](https://www.newegg.com/black-fractal-design-node-304-mini-itx-tower/p/N82E16811352027)|ITX, 14.7"x9.8"x8.3" ALT: Node 804 ($120), CM N400 ($80), [DIY NAS Case List](/wiki/storage#diy-nas-case-list)
CPU|Intel i3-12100 CPU, 60W|$115|[pcpartpicker](https://pcpartpicker.com/product/qrhFf7/intel-core-i3-12100-33-ghz-quad-core-processor-bx8071512100)|Passmark CPU Mark: [13000+](https://www.cpubenchmark.net/cpu.php?cpu=Intel+Core+i3-12100&id=4687). ALT: i5-12400 ($135)
MOBO|ASRock B760M-ITX/D4|$150|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&s=40&f=8&sort=price&page=1)|ALT: [B660M/B760M uATX mobo](https://pcpartpicker.com/products/motherboard/#f=7&sort=price&xcx=0&s=40&K=5,13)
MEM|Team T-Force Vulcan Z 32GB 2x16GB DDR4-3200|$50|[pcpartpicker](https://pcpartpicker.com/product/bcnypg/team-t-force-vulcan-z-32-gb-2-x-16-gb-ddr4-3200-cl16-memory-tlzgd432g3200hc16fdc01)|ALT: Team T-Force Vulcan Z 16GB 2x8GB DDR4-3200 ($35)
STORAGE|PNY Attache 4 32GB USB Flash Drive (BOOT)|$12|[amazon](https://www.amazon.com/PNY-Attache-Drives-3-Pack-P-FD32GX3ATT4-GE/dp/B07YVY2H1J)| USB 2.0 for low heat/longevity
STORAGE|WD SN770 1TB NVMe M.2 SSD (APP/CACHE)|$70|[pcpartpicker](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e)|ALT: [SK Hynix P31 1TB](https://pcpartpicker.com/product/xNCFf7/sk-hynix-gold-p31-1-tb-m2-2280-pcie-30-x4-nvme-solid-state-drive-shgp31-1000gm-2)
STORAGE|3 x Seagate Exos X14 12TB HDD (DATA)|$540|[disctech](https://www.disctech.com/Seagate-Exos-X14-ST12000NM0538-12TB-3.5-LFF-6Gbps-7.2K-RPM-FastFormat-512e-Enterprise-SATA-Hard-Disk)| SEPARATE. ALT: [Ultrastar HC530 14TB](https://www.disctech.com/interface-types/SATA?order=relevance:asc&keywords=hc530) (better $/GB)
STORAGE|LSI 9207-8i, in IT/HBA mode|$40|[ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=9207+8i+%2Bcables&_sacat=0&LH_TitleDesc=0&_dmd=1&_stpos=80232-6476&_odkw=9201+%2B16i+%2Bcables&_osacat=0&_sop=15&LH_PrefLoc=2&_ipg=60&_sadis=15)|OPTIONAL. For more than 4xSATA ports/better controller support. ALT: [SATA card](https://www.amazon.com/dp/B0BNFBXBNS)
COOL|Noctua NH-U12S Redux CPU Cooler|$50|[pcpartpicker](https://pcpartpicker.com/product/vV7G3C/noctua-nh-u12s-redux-7075-cfm-cpu-cooler-nh-u12s-redux)|ALT: be quiet Pure Rock 2 ($40)
PSU|Corsair RM/CX 650-750W|$75|[pcpartpicker](https://pcpartpicker.com/products/power-supply/#xcx=0&th=1&A=500000000000,750000000000&p=1,3,2&sort=price&m=8,337,50,11,14,106,101,17,18,58,62,824,27,28,94,29,229,51,71,63,441,113,56,39,60&e=4,3,2,1)|ALT: EVGA/Seasonic
SOFTWARE|Unraid Starter - 6 device license|$50|[limetech](https://unraid.net/pricing)|
TOTAL||$672||

<!-- Sub-Section -->

<!-- ### $4000 Almost Ultimate NAS (126TB) + Media Server (59L) -->
### $1300 Almost Ultimate NAS / Media Server (59L)

If you have massive storage requirements now, or plan on in the future, and don't want to go hot-swap or rackmount, this build will fit the bill. 
The Meshify 2 case is quality and well-priced for 13xHDDs and has fan slots up front to cool your data HDDs sufficiently, as when maxed out they will 
collectively produce a lot of heat. See our [Storage Setup Guide](/wiki/storage#diy-nas-case-list) for additional case options.  

The CPU may seem meager, not being a K sku, but we don't need much power, we mostly want the iGPU for hardware media transcoding and the specced cooler is 
more than enough for this 65W CPU. If you opt for the 12600K, move up to the Peerless Assassin cooler.  

We use highly reliable, well-priced Seagate Exos HDDs here for our data. Alternatively, WD Ultrastar drives are just as good. Since this is the bulk of our 
cost, find the best price you can and, if you can, order from multiple vendors to get different batches of drives.  

We configure this build for 126TB of usable space with dual-parity protection (14TBx11 = 154TB total - 28TB parity = 126TB usable) to show the potential of what's possible. If you want to start with smaller-sized or a smaller number of drives and mix-and-match sizes later, you can do that, but your parity drive(s) should be as big as the largest usable data drive you plan on having. It is also not recommended to go over 6 usable data drives per parity drive.  

Keeping a backup of this much data would be a serious problem without building a second system to sync to, even if we do have a dual-parity protected array. 
If a backup is something you may want, consider splitting up the drives into 2 arrays. Such as 1 active array w/6 drives (5 usable+1 parity) and a backup 
array with 5 drives (5 usable+0 parity). Then sync the active array to the backup array nightly with something like rsync. With the configured drives, 
that'd give you 70TB usable and backed-up. If you wanted to make up for the lost usable space in such a configuration, you could go all the way up to 
20TB drives and have 100TB usable.  

For app/cache storage, such things as VMs, Docker data and media caching, we have 2 SSDs to create a 1TB parity-protected array (essentially a RAID1).  

Unraid will boot off the USB flash drive, so we have a reliable USB 2.0 one here, with backups.  

Lots of well-priced DDR5 RAM for VMs, Dockers and, if you so choose, Plex media transcoding in RAM.  

If you want a system with ECC memory and a workstation mobo, see our [pcpartpicker part list](https://pcpartpicker.com/list/yvMQ6Q).  

As a Plex server, with the purchased Plex Pass, you can transcode ~12x4k or 25x1080p transcodes concurrently on the CPU's iGPU. Without a Plex Pass, 
expect 8x1080p streams with CPU software transcoding. <!-- For more transcodes, add a used [Quadro P5000](https://www.elpamsoft.com/?p=Plex-Hardware-Transcoding) dGPU (11x4k,22x1080p) ($300). -->

The LSI HBA adapter has 8 ports for SATA drives. You can use the SATA ports on the motherboard for your HDDs, then add on the HBA when you outgrow those, or vice-versa.  

For the motherboard, in theory any Z690/Z790 ATX/uATX board will work with 2 x16 slots, if you want to have support for a potential dGPU upgrade. We need at least 1 slot for our LSI HBA Adapter to connect our data drives to and then 1 slot for a potential dGPU. On the chosen board we also have dual LAN. 

The PSU wattage may seem overkill, but we again plan for any upgrades, CPU, GPU, etc.. and remember that each HDD can pull 10W on spin-up.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|	Fractal Design Meshify 2			|	$130	|	[pcpartpicker](https://pcpartpicker.com/product/jqTzK8/fractal-design-meshify-2-atx-mid-tower-case-fd-c-mes2a-02)	|[[specs](https://www.fractal-design.com/products/cases/meshify/meshify-2/black-tg-dark-tint/)]. ALT: Fractal Design Define 7 ($160)
CPU		|	Intel i5-12500 6C/12T CPU (65W)			|	$200	|	[pcpartpicker](https://pcpartpicker.com/product/hvC48d/intel-core-i5-12500-3-ghz-6-core-processor-bx8071512500)	|ALT: [Intel i5-12600k](https://pcpartpicker.com/product/BB4Ycf/intel-core-i5-12600k-37-ghz-6-core-processor-bx8071512600k)
MOBO		|ASRock Z690 Taichi DDR5 ATX			|	$200	|	[pcpartpicker](https://pcpartpicker.com/product/VVC48d/asrock-z690-taichi-atx-lga1700-motherboard-z690-taichi)	|ALT: [Other DDR5 Motherboards](https://pcpartpicker.com/products/motherboard/#h=2,8&K=6,13&sort=price&c0=1x2500-1x1000,1x2500&xcx=0&s=40&f=2,7&mt=ddr5)
MEM		|	G.Skill Ripjaws S5 64GB (2x32GB) DDR5-6000	|	$160	|	[pcpartpicker](https://pcpartpicker.com/product/6npQzy/gskill-ripjaws-s5-64-gb-2-x-32-gb-ddr5-6000-cl36-memory-f5-6000j3636f32gx2-rs5k)	| ALT: [32GB (2x16GB) DDR5](https://pcpartpicker.com/products/memory/#xcx=0&Z=32768002&sort=price&ff=ddr5&S=5600,8400)
STORAGE		|	PNY Attache 4 32GB USB Flash Drive (BOOT)	|	$12 |	[amazon](https://www.amazon.com/PNY-Attache-Drives-3-Pack-P-FD32GX3ATT4-GE/dp/B07YVY2H1J)		| USB 2.0 for low heat/longevity
STORAGE		|	2x SK Hynix P41 1TB NVMe M.2 SSD (APP/CACHE)	|	$160	|	[pcpartpicker](https://pcpartpicker.com/product/sw2WGX/sk-hynix-platinum-p41-1-tb-m2-2280-pcie-40-x4-nvme-solid-state-drive-shpp41-1000gm-2)	|ALT: Samsung 990 Pro
STORAGE		|	11x Seagate Exos X16 14TB SATA HDD (DATA)		|	$2300	|	[disctech](https://www.disctech.com/data-storage/internal-storage/sata-hard-drives/capacity/14TB/manufacturer/Seagate?order=onlinecustomerprice:asc)	| SEPARATE. ALT: WD Ultrastar DC HC530 14TB
STORAGE		|	LSI 9207-8i Adapter (x8) + Cables, in IT/HBA mode	|	$40	|	[ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=9207+8i+%2Bcables&_sacat=0&LH_TitleDesc=0&_dmd=1&_stpos=80232-6476&_odkw=9201+%2B16i+%2Bcables&_osacat=0&_sop=15&LH_PrefLoc=2&_ipg=60&_sadis=15)	|ALT: [Adaptec ASR 71605 (x16)](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=adaptec+asr+71605+%2Bcables&_sacat=0&LH_TitleDesc=0&_odkw=Adaptec+ASR+71605&_osacat=0) ($50)
STORAGE          |       SATA Power Splitter Cables                                  |       $15  |       [amazon](https://www.amazon.com/Cable-Matters-Pack-Power-Splitter/dp/B012BPLW08)   |  
COOL		|	Arctic P14 PWM 140 mm Fan (FRONT)		|	$15	|	[amazon](https://www.amazon.com/dp/B07GZJY4TM?tag=pcpapi-20&linkCode=ogi&th=1&psc=1)		|
COOL		|	Thermalright Silver Soul 135 CPU Cooler			|	$35	|	[pcpartpicker](https://pcpartpicker.com/product/sRPQzy/thermalright-silver-soul-135-82-cfm-cpu-cooler-silver-soul-135-black-d2)	|ALT: Thermalright Peerless Assassin 120 SE ($40)
PSU		|	SeaSonic FOCUS Plus 750 Gold ATX PSU	|	$100	|	[pcpartpicker](https://pcpartpicker.com/product/64cMnQ/seasonic-focus-plus-gold-750w-80-gold-certified-fully-modular-atx-power-supply-ssr-750fx)	|ALT: [Other PSUs](https://pcpartpicker.com/products/power-supply/#xcx=0&A=750000000000,2000000000000&p=1,2&sort=price&D=7,20&e=5,4&m=337,50,11,14,229,71,63,441&th=1)
SOFTWARE	|	Unraid Unleashed - Unlimited device license		|	$110	|	[limetech](https://unraid.net/pricing)	|
SOFTWARE	|	Plex Media Server				|	$0	|	[Plex](https://www.plex.tv/downloads)		|Free
LICENSE		|	Plex Pass					|	$120	|	[Plex](https://www.plex.tv/plex-pass/)		|Lifetime cost or $40/year, $5/month.
TOTAL		|							|	$1297	|			|

<!-- Sub-Section -->

### $150 Large NAS / Utility Server (36L) - Used

A step up from the previous Medium build in internal capacity, but still used hardware, so similar in cost. It's large and an old arch, but good for mass storage and other lightweight duties vs the cost of a pre-built NAS.  

This is a setup with hardware off ebay using the old Ivy Bridge architecture. Plenty of power for NAS and utility task duties. Yes, it can be used as a Plex media server as well for its [Direct Play](https://support.plex.tv/articles/200430303-streaming-overview/) 
and H264 transcode ability (look at the Dell 3620 option in the previous used build for 4k/HEVC transcoding), but that's not our primary focus here. Our focus is internal storage capacity.  

This can fit 6x3.5 HDDs (using 3x3.5" and 3x5.25" mounts) officially. Since it has 6x SATA ports, you'll ideally use 1x for a SATA SSD for an os/app/cache drive and the other 5x for any data HDDs. For raw storage this has you in the realm of 40TB-120TB of storage potential. If you get creative, you can fit 8x 3.5" drives along with a [9207-8i SAS->SATA HBA](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=9207+8i&_sacat=0&LH_TitleDesc=0&_odkw=hp+cmt&_osacat=0&LH_PrefLoc=2) or [SATA card](https://www.amazon.com/dp/B0BNFBXBNS), and [SATA Power Splitters](https://www.amazon.com/Cable-Matters-Power-Y-Splitter-Inches/dp/B00V6QA65G).  

If you go with an i5/i7 version, you'll get non-ECC memory. With a Xeon version you can use ECC memory, which is better for data integrity. 
You should also have a battery-backup UPS as well if you really care about data integrity.  

If you want ease-of-use management, spend the extra $$ on [Unraid](https://unraid.net) as your OS and its web-based system for VMs and Docker containers. Otherwise, look at TrueNAS or just use Linux/[OpenMediaVault](https://www.openmediavault.org/) and 
either set up drives as individual volumes or use [mergerFS](https://github.com/trapexit/mergerfs/wiki).  

If you can't find a HP Z220 CMT setup, you can alternatively go with a HP Z210 CMT.  

See our [Storage Setup Guide](/wiki/storage) for more information on software and drives.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
PC			|HP Z220 CMT Workstation				|$120		|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2047675.m570.l1313&_nkw=HP+Z220+CMT&_sacat=0)	| ALT: HP Z210 CMT
CPU			|Intel i5/i7-3xxx, Xeon E3-1xxx			|Included	|	NA			|	65-77 W, 4C/4T, PASSMARK: 4500
MEM/STORAGE	|8GB DDR3 RAM, 500GB (varies) HDD		|Included	|	NA			|	Xeon: [ECC](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=ecc+8gb+12800+unbuffered+dimm&_sacat=0&LH_TitleDesc=0&_odkw=ecc+8gb+12800+unbuffered+dimm&_osacat=0&LH_PrefLoc=2), i3/i5: non-ECC
STORAGE		|512GB 2.5" SATA SSD (OS/APP/CACHE)		|$30		|	[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=480000000000,22000000000000&t=0&sort=price&c1=di_sata.60)		| 
STORAGE		|4-24TB HDD - (DATA) |Varies		|	NA			|	[NAS Drive List](/wiki/storage#hard-drives)
OS			|Unraid/Ubuntu 22/OMV/Windows			|$0			|	[Ubuntu](https://ubuntu.com/download)		|	Windows 10 usually included
SOFTWARE	|Unraid Starter - 6 device license				|$50		|	[limetech](https://unraid.net/pricing)		|	OPTIONAL
TOTAL		|										|$150		|	NA			|

<!-- $300-$500: NEW, PRE-BUILT, MEDIA SERVER, INTERNAL 3.5" STORAGE: HP TP01,Dell 3891/3910,Intel 10th-12th gen,1xHDDs (official) 3xHDDs (un-official) w/sata power splitter+creative hdd mounting. [Ebay](https://www.ebay.com/sch/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=\(hp%2Cdell\)+\(tp01%2C3891%2C3910\)+\(i3%2Ci5%2Ci7\)&_sacat=179&LH_BIN=1&LH_TitleDesc=0&_sop=15&LH_PrefLoc=2&LH_ItemCondition=1500%7C1000) -->

<!-- Section -->

## Gaming Emulation builds

<!-- Sub-Section -->

### $100 720p/1080p Gaming Emulation Box (1.2L)

This is a good, small (Micro/USFF) emulation box for NES/SNES, Game Gear, Sega Master/Saturn/Dreamcast, PSP/PS1, N64/Gamecube, AtomisWave.  
3DS, PS2 and anything greater will struggle a bit, depending on the game. Check [ETA Prime's reviews](https://www.youtube.com/watch?v=XONKVZf0m6o). If you want to run those, move up to a i5-8500 SFF and low profile Nvidia GT 1030 GDDR5 used off ebay for $70 more; if you need to stay in the Micro/USFF form-factor, look at [AMD-based pre-builts](https://www.ebay.com/sch/179/i.html?_from=R40&_nkw=%283200ge%2C3400ge%2C2400ge%2C3200ge%29&LH_TitleDesc=0&LH_BIN=1&_sop=15&_udhi=150%29+%28%24100%29+OR+%3E%3D+%5BJ4125+Mini+PC%5D%28https%3A%2F%2Fwww.amazon.com%2FNucBox-Windows-Computer-Intel-J4125%2Fdp%2FB092JFVX2Z) ($175).  
This is not for anything like PS3, CEMU, or anything >= Xbox  

Make sure to get one with 2x4GB sticks of RAM, not a single stick.  

For your frontend, Batocera (linux) and LaunchBox/BigBox (windows) are good choices. Solus is good if you want a fully fledged linux interface.  

Will handle 1080p video duties fine

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|HP/Dell/Lenovo	|	$90	|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400t%2Ci5-8500t%29&_sacat=179&_fsrp=1&_odkw=%28hp%2Cdell%2Clenovo%29+%28i5-8400t%2Ci5-8500t%2Ci5-7400t%2Ci5-7500t%29&_osacat=179&LH_BIN=1&_sop=15&LH_PrefLoc=2&_udhi=150)	|	Prodesk G4, Optiplex 3060/5060/7060, Thinkcentre M720q/M920q
CPU/GPU		|Intel i5-8500T	|	Included|	NA|		ALT: i5-7500T
MEM			|2x4GB (8GB) DDR4|	Included|	NA|		NA
STORAGE		|120-500GB HDD/SSD		|	Included|	NA|		ALT: 2.5"/M.2 SSD ($30)
ACCESSORY	|DP to HDMI Cable	|	$10	|	[Amazon](https://www.amazon.com/Amazon-Basics-Uni-Directional-DisplayPort-Display/dp/B015OW3M1W/)	| 1080p/60, 4k/30
TOTAL		|				|	$100	||

<!-- Sub-Section -->

### $300 720p/1080p Gaming Emulation Box (12L)

Good for 720p internal resolution on emulators, [1080p up to Wii/Gamecube/PS2](https://www.youtube.com/watch?v=J97MxOr9hu0&t=11s). Less demanding PS3 games are possible, but you might have to take down to 720p.  

Will handle 4k video duties just fine.  

This is a bottom-barrel build, due to Micro-ATX motherboard being cheaper, CPU a tick slower, a larger case and a smaller SSD.  

For better quality parts, see ALT: notes, for a better case, motherboard and separate PSU. @$60 more. For more oomph, see the $500 build below.  

For an even smaller box, you could go with the Asrock Deskmini A300W/X300W case at 1.9L. Skip motherboard and change ram to DDR4-3200 2x8GB SO-DIMMS. $30 more.  

If you don't want to build, you can find [SFF/USFF pre-builts on Ebay with the Ryzen 2400G/3400G](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=%283400ge%2C2400ge%2C2400g%2C3400g%29&_sacat=179&LH_TitleDesc=0&_odkw=%283400ge%2C2400ge%29&_osacat=179&LH_BIN=1&_sop=15&_udhi=150%29+%28%24100%29+OR+%3E%3D+%5BJ4125+Mini+PC%5D%28https%3A%2F%2Fwww.amazon.com%2FNucBox-Windows-Computer-Intel-J4125%2Fdp%2FB092JFVX2Z) for around $200, sometimes cheaper.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE	|InWin Slim BL040 MicroATX case w/300W PSU			|$100		|[amazon](https://www.amazon.com/InWin-BL040-mATX-Desktop-Black/dp/B0964K2W4R)	|ALT: [Silverstone ML03b](https://pcpartpicker.com/product/bWR48d/silverstone-case-ml03b) (15.7L) ($95)/[Jonsbo C6](https://www.newegg.com/p/2AM-006A-000C4) (15.8L) ($60)
PSU		|Included							|$0		|	|ALT: [EVGA BQ 500W](https://pcpartpicker.com/product/8P7CmG/evga-bq-500w-80-bronze-certified-semi-modular-atx-power-supply-110-bq-0500-k1) ($60)
CPU		|AMD Ryzen 5500GT APU (65W)				|$110		|[pcpartpicker](https://pcpartpicker.com/product/VcvD4D/amd-ryzen-5-5500gt-36-ghz-6-core-processor-100-100001489box)	|ALT: [Ryzen 3400G - Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=3400g&_sacat=0&LH_BIN=1&_sop=15) ($75)
MOBO	|MSI A520M-A PRO MicroATX		|$70		|[pcpartpicker](https://pcpartpicker.com/product/nZTzK8/msi-a520m-a-pro-micro-atx-am4-motherboard-a520m-a-pro)	|ALT: 3400G: [MSI A320M PRO](https://pcpartpicker.com/product/mB4BD3/msi-a320m-a-pro-micro-atx-am4-motherboard-a320m-a-pro) ($80)
MEM		|Silicon Power Gaming 2x8GB DDR4-3200		|$30		|[pcpartpicker](https://pcpartpicker.com/product/P4FKHx/silicon-power-sp016gxlzu320bdaj5-16-gb-2-x-8-gb-ddr4-3200-cl16-memory-sp016gxlzu320bdaj5)	|ALT: Deskmini: [2x8GB DDR4-3200 SODIMMS](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr4&ff=ddr4_sodimm&sort=price&S=2666,8000&Z=16384002)
STORAGE	 	|WD SN580 250GB NVMe M.2 SSD					|$30		|[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#t=0&A=250000000000,22000000000000&f=122080&D=1&sort=price&page=1)	|ALT: WD Black SN580 500 GB M.2 ($40)
TOTAL	|								|$330	|	|

<!-- Sub-Section -->

### $500 720p/1080p Gaming Emulation Box (3.3L)

This just uses a Ryzen 8500G APU, no dedicated GPU which is fine for light gaming and 4k video. A 8600G would give even better gaming performance.  

Emulation: You should be able to play at 45-60 fps for most everything at 720p internal resolution and <= 32-bit systems at 1080p. Demanding platforms (like Xbox 360) and 64-bit titles, like BoTW, expect <= 30 fps@1080p. You can push Wii/PS3 to 60 fps@1080p, w/BoTW up to 50 fps at the extreme limits of a 8600G. Check out ETA PRIME's [8600G](https://www.youtube.com/watch?v=puKstrlDLOI) reviews for actual game data.  

Gaming: Expect 50 fps@1080p Med for most games, with a 8600G pushing that up to 60 fps@1080p Med sans harder games like Doom Eternal/Cyberpunk/etc.. which you'll have to run Low w/FSR upscaling.

For an even smaller box, you could go with the Asrock Deskmini X600 at 1.9L as shown in the Notes column. And it comes out to about $45 cheaper since you don't need to buy a motherboard. Everything else stays the same.  

For a fanless build, with same perf., for $250 more, see build in HTPC section above

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE			|Inwin Chopin/BQ656										|$100		|[amazon](https://www.amazon.com/InWin-BQ656-Mini-ITX-Internal-Optical/dp/B0CXLTTXM9)		|8.6"x9.6"x3.3" ALT: Deskmini X600 ($170) (1.9L)
MOBO			|ASRock A620I Lightning Wifi						|$130	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#f=8&sort=price&xcx=0&s=41)		|ALT: Deskmini: Not applicable
CPU				|AMD Ryzen 8500G APU				|$150	|[pcpartpicker](https://pcpartpicker.com/product/y3XV3C/amd-ryzen-5-8500g-41-ghz-6-core-processor-100-100000931box)		|ALT: [Ryzen 8600G](https://pcpartpicker.com/product/QqyH99/amd-ryzen-5-8600g-43-ghz-6-core-processor-100-100001237box)
MEM		|Crucial Classic 2x8GB DDR5-5600		|$47		|[pcpartpicker](https://pcpartpicker.com/product/y4BzK8/crucial-classic-16-gb-2-x-8-gb-ddr5-5600-cl46-memory-ct2k8g56c46u5)	|ALT: Deskmini: [2x8GB DDR5-5600 SODIMMS](https://pcpartpicker.com/products/memory/#xcx=0&b=ddr5&Z=16384002&sort=price&ff=ddr5_sodimm)
STORAGE			|WD Black SN770 500GB NVMe M.2 SSD TLC			|$45		|[pcpartpicker](https://pcpartpicker.com/product/nWC48d/western-digital-500-gb-m2-2280-nvme-solid-state-drive-wds500g3x0e)		|ALT: [1TB M.2 SSD](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e) ($75)
COOL			|Thermalright AXP90-X53 CPU Cooler							|$25		|[pcpartpicker](https://pcpartpicker.com/product/3g7G3C/thermalright-axp90-x53-4258-cfm-cpu-cooler-axp90-x53)		|
TOTAL			|												|$497	|		|

<!-- Sub-Section -->

### $650 1080p Gaming Emulation Box (12L)

You should be able to play 60+ fps for most everything  

Will handle 4k video duties just fine.  

For a SFF case, see the VR builds  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|Silverstone ML08				|$120		|[pcpartpicker](https://pcpartpicker.com/product/bvfmP6/silverstone-case-sstml08b)		|14.57" x 14.96" x 3.43" ALT: ML07
MOBO		|ASRock B760M-ITX/D4			|$145	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&s=40&f=8&sort=price&page=1)	|
CPU			|Intel i5-12400F, 65W						|$115	|[pcpartpicker](https://pcpartpicker.com/product/pQNxFT/intel-core-i5-12400f-25-ghz-6-core-processor-bx8071512400f)	|ALT: Intel i5-12100F
GPU			|Nvidia GTX 1660 Super		|$110	|[ebay](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=gtx+1660+super&_sacat=0&LH_TitleDesc=0&rt=nc&_odkw=rtx+2060&_osacat=0&LH_BIN=1&_sop=15)	|ALT: 1440p: GTX 1070
MEM			|Corsair Vengeance 16GB 2x8GB DDR4-3200	|$40		|[pcpartpicker](https://pcpartpicker.com/product/p6RFf7/corsair-memory-cmk16gx4m2b3200c16)	|
STORAGE		|WD Black SN580 500GB NVMe M.2 SSD TLC	|$45		|[pcpartpicker](https://pcpartpicker.com/product/kHRwrH/western-digital-blue-sn580-500-gb-m2-2280-pcie-40-x4-nvme-solid-state-drive-wds500g3b0e)	|ALT: [1TB M.2 SSD](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e) ($70)
PSU			|EVGA Supernova GM 550W Full Modular SFX			|$90		|[pcpartpicker](https://pcpartpicker.com/product/QgyV3C/evga-supernova-gm-550w-80-gold-certified-fully-modular-sfx-power-supply-123-gm-0550-y1)	|ALT: [SFX PSUs](https://pcpartpicker.com/products/power-supply/#sort=price&th=5&p=1,3,2&e=6,5,4,2,1)
TOTAL		|									|$665	|	|

<!-- Sub-Section -->

### $800 4k Gaming Emulation Box (19.5L)

You should be able to play 60+ fps for most everything, sans some demanding titles, like BoTW (60fps), Skate 3 (60fps), etc..  

Will handle 4k video duties just fine.  

For a SFF case, see the VR Box builds  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE|Fractal Design Node 304|$100|[newegg](https://www.newegg.com/black-fractal-design-node-304-mini-itx-tower/p/N82E16811352027)|ITX, 14.7"x9.8"x8.3" ALT: Thermaltake Core V1 ($51)
MOBO		|Asrock B760M-ITX/D4				|$150	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&s=40&f=8&sort=price&page=1)		|ALT: ASRock B550M-ITX/ac ($135)
CPU			|Intel i5-12400F								|$120	|[pcpartpicker](https://pcpartpicker.com/product/pQNxFT/intel-core-i5-12400f-25-ghz-6-core-processor-bx8071512400f)		|ALT: AMD Ryzen 5700x ($130)
GPU			|Nvidia RTX 2060				|$160	|[ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=rtx+2060&_sacat=0&_sop=15&rt=nc&LH_BIN=1)		|ALT: AMD RX 5700 XT
MEM			|G.Skill Ripjaws V 16GB 2x8GB DDR4-3600 CL18				|$40		|[pcpartpicker](https://pcpartpicker.com/product/n6RgXL/gskill-ripjaws-v-16-gb-2-x-8-gb-ddr4-3600-memory-f4-3600c18d-16gvk)		|ALT: Corsair Vengeance LPX 2x8GB DDR4-3600
STORAGE		|WD SN770 1TB NVMe M.2 SSD TLC			|$70	| [pcpartpicker](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e)		|
COOL		|Noctua NH-U12S Redux CPU Cooler					|$50		|[pcpartpicker](https://pcpartpicker.com/product/vV7G3C/noctua-nh-u12s-redux-7075-cfm-cpu-cooler-nh-u12s-redux)		|ALT: [Thermalright Silver Soul 135](https://pcpartpicker.com/product/c3pzK8/thermalright-silver-soul-135-82-cfm-cpu-cooler-ss135) ($40)
PSU			|EVGA G5 Full-Modular 650W ATX			|$80	|[pcpartpicker](https://pcpartpicker.com/products/power-supply/#xcx=0&sort=price&th=1&e=6,5,4,3,2,1&p=1,2)		|ALT: Corsair CX650M ($90)
TOTAL		|											|$770	|		|

<!-- Section -->

## Gaming builds

<!-- Sub-Section -->

### 1080p Gaming Steam Box - USED

This budget gaming build runs on Manjaro Linux w/Steam.  
It's good for 1080p, High @ 60 fps+ on normal games, Medium @ 45-60 fps on AAA games.  
It uses a Pre-built PC and GPU from Ebay.  
Make sure you pick a GPU with a 6-pin (not 8) power connector and a PC with 2 sata connectors free for GPU power. Any Dell/HP/Lenovo MT/tower from the search with an i7-6700 - i5-8500 is fine. You can usually find one with an M.2 SSD so you don't have to purchase one separately like listed below.  
Manjaro linux OS is free and fine for Steam use and comes pre-installed with it. Simply download the Manjaro KDE Plasma iso, write it to the USB flash drive with Etcher, boot from it and install to your SSD. Install the nvidia non-free/proprietary drivers at install or [later](https://wiki.manjaro.org/index.php/Configure_Graphics_Cards#Identifying_Available_Drivers), then Enable Steam Play and Proton in the Compatability preferences of the Steam client.  
Alternatively, you can run Windows if you want, and you have an activation key.  

PART			|BRAND/MODEL												|	PRICE	|	VENDOR	|	NOTES
:--|:--|:--|:--|:--
CASE/CPU/MEM	|Dell/HP/Lenovo Mini Tower pre-built w/8GB RAM	|	$100	|	[Ebay](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28dell%2Chp%2Clenovo%29+%28mt%2Ctower%29+%28i7-6700%2Ci7-7700%2Ci5-8500%2Ci5-8400%29&_sacat=179&LH_TitleDesc=0&_sop=15&rt=nc&LH_All=1)	|	ALT: [i5-8500](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28dell%2Chp%2Clenovo%29+%28mt%2Ctower%29+%28i7-6700%2Ci7-7700%2Ci5-8500%2Ci5-8400%29&_sacat=179&LH_TitleDesc=0&_sop=15&rt=nc&LH_All=1) ($110)
GPU				|Nvidia GTX 1060 6GB w/6-pin								|	$75	|	[Ebay](https://www.ebay.com/sch/27386/i.html?_fsrp=1&rt=nc&_from=R40&_nkw=gtx+1060+%226GB%22&LH_BIN=1&_sacat=27386&_sop=15&LH_ItemCondition=1000%7C1500%7C2020%7C3000)	|	ALT: Nvidia GTX 1650 Super 6-pin ($100)
STORAGE		|512GB M.2 NVMe SSD										|	$30		|	[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&sort=price&A=450000000000,525000000000&D=1&f=122080)	|	ALT: [2.5" Version](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&sort=price&A=450000000000,525000000000&f=3&t=0) ($25)
STORAGE		|16GB+ USB flash drive												|	$7		|	[Amazon](https://www.amazon.com/SanDisk-Ultra-Flash-Drive-100MB/dp/B00DQG9DDU)	|	For Linux install
ADAPTER			|SATA dual to pcie 6-pin adapter							|	$7		|	[Amazon](https://www.amazon.com/Power-Express-Video-Cable-Adapter/dp/B007Y91B80)	|	
ACCESSORY	|HDMI to HDMI Cable						|$10			|	[Amazon](https://www.amazon.com/Monoprice-115428-Certified-Premium-18Gbps/dp/B01GCGKI3O)	| HDMI 2.0 - 6 Ft
OS				|Manjaro Linux w/KDE Plasma									|	$0		|	[Download](https://manjaro.org/products/download/x86)	|	
SOFTWARE		|Etcher ISO writer											|	$0		|	[Download](https://www.balena.io/etcher/)	|	
SOFTWARE		|Steam + Proton Experimental								|	$0		|	NA		|	
TOTAL			|															|	**$229**	|			|	

<!-- Sub-Section -->

### 1080p Gaming Box (8.8L)

This is a straight up gaming build for 1080p with High settings, averaging about 90-100 fps which is good for a 120 Hz TV.  
It simplifies things by including the motherboard and PSU. If you want a low profile case or more flexibility, look at the ALT: config with a Silverstone ML-07 case instead (you'll have to add an [ITX mobo](https://pcpartpicker.com/products/motherboard/#xcx=0&s=33&f=8&sort=price&page=1) and [SFX PSU](https://pcpartpicker.com/products/power-supply/#th=5&sort=price&page=1&A=450000000000,2050000000000)).  

PART			|BRAND/MODEL			|	PRICE	|	VENDOR	|	NOTES
:--|:--|:--|:--|:--
CASE/MOBO/PSU		|Asrock DeskMeet X300W w/500W PSU					|$170	|[newegg](https://www.newegg.com/asrock-deskmeet-x300w-b-bb-box-us/p/N82E16856158083)	|6.6" (W) x 9.3" (D) x 8.7" (H), [specs](https://www.asrock.com/nettop/AMD/DeskMeet%20X300%20Series/index.asp#Specification). ALT: ML-07+ITX+SFX
CPU	|	AMD Ryzen 5700X (65W)				|	$150	|pcpartpicker	|ALT: AMD Ryzen 5700X3D
GPU	|	AMD RX 6600 8GB			|	$200	|[pcpartpicker](https://pcpartpicker.com/products/video-card/#xcx=0&c=511&L=69000000,200000000&sort=price&page=1)	|<= 200 mm (L). ALT: AMD RX 7600 8GB
MEM	|	Teamforce Vulcan Z 32GB 2x16GB DDR4-3600	|	$55	|[pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&ff=ddr4&S=3600,3733&Z=32768002&sort=price)	|ALT: 16 GB 2x8GB ($35)
STORAGE	|	WD SN580 1TB M.2 (OS/GAMES)	|	$60	|pcpartpicker	|
COOL		|Thermalright AXP90-X47 CPU Cooler, 47mm			|	$25		|[pcpartpicker](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=14000000,47000000&c=33&W=0&sort=price&page=1)	|Quieter than stock cooler. *ML-07*: [AXP120-X67](https://pcpartpicker.com/products/cpu-cooler/#xcx=0&H=66500000,72600000&sort=price&m=113)
TOTAL	|						|	**$660**	|	

<!-- Sub-Section -->

### 1440p Gaming Box (14L)

This is a straight up gaming build for 1440p with High settings, averaging about 90-100 fps which is good for a 120 Hz TV.  
It's low profile so is good for a media cabinet. If you can handle more height or want to beef up the perf, look at the ALT: notes. 

PART			|BRAND/MODEL			|	PRICE	|	VENDOR	|	NOTES
:--|:--|:--|:--|:--
CASE	|	Silverstone Milo Z/ML-07		|	$105	|pcpartpicker	|15" (W)x4.1" (H)x13.8" (D). ALT: Silverstone GD-11 (6.9" (H), 30L)
CPU	|	AMD Ryzen 5700X3D (105W)			|	$200	|pcpartpicker	|ALT: AMD Ryzen 7600X3D
GPU	|	AMD RX 6750 XT 12GB			|	$310	|[pcpartpicker](https://pcpartpicker.com/products/video-card/#c=523,495&xcx=0&sort=price)	|ALT: AMD RX 7800 XT 16 GB
MOBO	|	ASRock B550M-ITX/ac		|	$135	|[pcpartpicker](https://pcpartpicker.com/products/motherboard/#xcx=0&f=8&c=147,124,133,145,123,132,138&sort=price)	|ALT: Gigabyte B650 GAMING X AX ATX
MEM	|	Teamforce VulcanZ 32GB 2x16GB DDR4-3600	|	$55	|[pcpartpicker](https://pcpartpicker.com/products/memory/#xcx=0&ff=ddr4&S=3600,3733&Z=32768002&sort=price)	|ALT: G.Skill Flare S5 2x16GB 32GB DDR5-6000
STORAGE	|	WD SN770 500GB M.2 (OS)	|	$50	|[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&D=1&A=450000000000,525000000000&sort=price&page=1)	|ALT: WD SN770 1TB M.2 (OS)
STORAGE	|	WD SN770 2TB M.2 (GAMES)	|	$120	|[pcpartpicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&D=1&A=1800000000000,2048000000000&sort=price&t=0)	|
PSU	|	Cooler Master V 850W SFX		|	$105	|[pcpartpicker](https://pcpartpicker.com/products/power-supply/#xcx=0&th=5&p=1,2&A=550000000000,2050000000000&sort=price&page=1)	|ALT: Corsair RM650x (2021) ATX
COOL	|	Thermalright AXP120-X67	CPU Cooler	|	$35	|pcpartpicker	|ALT: Thermalright Silver Soul 135 (Air) / Arctic Liquid Freezer II 240 (AIO)
TOTAL	|						|	**$1115**	|	

<!-- Section -->

## VR builds

<!-- Sub-Section -->

### $800 VR Box (11.5L)

The Silverstone case is a very good value, and does its job. Yes, it's no fancy Louqe Ghost, but neither is the price.  

We do go with a small SFX PSU here for more room, and it's not much more than a good full modular ATX PSU.  

You can also add a 3.5" HDD for an HTPC variation of this build, as long as you stick with the SFX PSU and the 120mm AIO. Any bigger and you run out of room quickly, especially for cables.  

You can however go with the thicker H80i AIO if you want to beef up your CPU cooling with an extra fan, though it isn't required. If you're not keen on AIO cooling, then a Noctua NH-L12S will fit fine with the SFX PSU.  

For CPU/MOBO you can replace AMD Ryzen with Intel i5-12400F/B660, if availability is a problem  

We chose a pretty small GPU here, but you can just as easily choose one all the way up to 270mm in length, but still dual-slot. The Radeon RX 6600/RTX 2060 is good for 1080p VR, but expect to jump to the RX 6650 XT/RTX 2060 Super or higher for 1440p.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|SilverStone SG13B										|$65			|[pcpartpicker](https://pcpartpicker.com/product/WG2bt6/silverstone-sg13-v2-mini-itx-tower-case-sg13b-usa)	|11.2" x 8.7" x 7.1"
MOBO		|ASRock B550M-ITX/ac					|$130			|[pcpartpicker](https://pcpartpicker.com/product/G6VG3C/asrock-b550m-itxac-mini-itx-am4-motherboard-b550m-itxac)	|ALT: [ASrock Fatal1ty B450 Gaming-ITX/ac](https://pcpartpicker.com/product/N4jJ7P/asrock-fatal1ty-b450-gaming-itxac-mini-itx-am4-motherboard-b450-gaming-itxac) ($150)
CPU			|AMD Ryzen 5600								|$120			|[pcpartpicker](https://pcpartpicker.com/product/PgcG3C/amd-ryzen-5-5600-36-ghz-6-core-processor-100-100000927box)	|ALT: Ryzen 5500
GPU			|AMD Radeon RX 6600	|$180		|[pcpartpicker](https://pcpartpicker.com/products/video-card/#sort=price&c=436,511,509&L=69000000,271000000)|ALT: Nvidia RTX 2060 ($200)
COOL		|Cooler Master MasterLiquid ML120L 120mm AIO				|$80		|[pcpartpicker](https://pcpartpicker.com/product/4TpmP6/cooler-master-masterliquid-ml120l-rgb-v2-6559-cfm-liquid-cpu-cooler-mlw-d12m-a18pc-r2)	|ALT: Corsair H60/H80i 120mm AIO ($80/$120), Noctua NH-L12S ($50)
MEM			|Corsair Vengeance 16GB 2x8GB DDR4-3200					|$40			|[pcpartpicker](https://pcpartpicker.com/product/p6RFf7/corsair-memory-cmk16gx4m2b3200c16)	|
STORAGE		|WD SN770 1TB NVMe M.2 SSD TLC					|$70		|[pcpartpicker](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e)	|ALT: WD SN850X 1TB M.2 ($75)
PSU			|Corsair CX650M (2021) 650W ATX				|$80			|[pcpartpicker](https://pcpartpicker.com/product/x96p99/corsair-cx650m-2021-650-w-80-bronze-certified-semi-modular-atx-power-supply-cp-9020221-na)	|ALT: [EVGA SuperNOVA 550 GM SFX](https://pcpartpicker.com/product/QgyV3C/evga-supernova-gm-550w-80-gold-certified-fully-modular-sfx-power-supply-123-gm-0550-y1) ($110)
TOTAL		|													|$765		|	|

<!-- Sub-Section -->

### $850 VR Box - Sandwich Case Variation (9.7L)

The $800 VR Box with a Geeek sandwich case. A little bit smaller than the SG13B.  

This changes the CPU cooler, PSU and fan compatibility. We can also use a longer GPU.  

For CPU/MOBO you can replace AMD with Intel i5-12400F/B660, if availability is a problem  

The Radeon RX 6600/RTX 2060 is good for 1080p VR, but expect to jump to the RX 6650 XT/RTX 2060 Super or higher for 1440p.  

PART|BRAND/MODEL|PRICE|VENDOR|NOTES
:--|:--|:--|:--|:--
CASE		|Geeek A50 Plus + PCIe riser cable					|$89				|[Geeek](https://www.geeekstore.com/shop/a50-plus-mini-itx-case/)	|13" x 5.5" x 8.4" ALT: Geeek A60 Plus ($99)
MOBO		|ASRock B550M-ITX/ac					|$130			|[pcpartpicker](https://pcpartpicker.com/product/G6VG3C/asrock-b550m-itxac-mini-itx-am4-motherboard-b550m-itxac)	|ALT: [ASrock Fatal1ty B450 Gaming-ITX/ac](https://pcpartpicker.com/product/N4jJ7P/asrock-fatal1ty-b450-gaming-itxac-mini-itx-am4-motherboard-b450-gaming-itxac) ($150)
CPU			|AMD Ryzen 5600								|$120			|[pcpartpicker](https://pcpartpicker.com/product/PgcG3C/amd-ryzen-5-5600-36-ghz-6-core-processor-100-100000927box)	|ALT: Ryzen 5500
GPU			|AMD Radeon RX 6600	|$180		|[pcpartpicker](https://pcpartpicker.com/products/video-card/#sort=price&c=436,511,509&L=69000000,304000000)|ALT: Nvidia RTX 2060 ($200)
MEM			|Corsair Vengeance 16GB 2x8GB DDR4-3200					|$40			|[pcpartpicker](https://pcpartpicker.com/product/p6RFf7/corsair-memory-cmk16gx4m2b3200c16)	|
STORAGE		|WD SN770 1TB NVMe M.2 SSD TLC					|$70		|[pcpartpicker](https://pcpartpicker.com/product/YVytt6/western-digital-1-tb-m2-2280-nvme-solid-state-drive-wds100t3x0e)	|ALT: WD SN850X 1TB M.2 ($75)
COOL		|Thermalright AXP90-X47 CPU cooler 						|$35				|[pcpartpicker](https://pcpartpicker.com/product/7GTp99/thermalright-axp90-x47-black-4258-cfm-cpu-cooler-axp90-x47-black)	|ALT: ID Cooling IS-50X/55 ($30)
COOL		|Noctua NF-A9x14 92mm Case fans 3x				|$60				|[Quietpc](https://www.quietpc.com/nf-a9x14-hs-pwm-ch-bk-s)	|2x is ok too for less noise, +4-5C temp
PSU			|EVGA SuperNOVA 550 GM SFX				|$110			|[pcpartpicker](https://pcpartpicker.com/product/QgyV3C/evga-supernova-gm-550w-80-gold-certified-fully-modular-sfx-power-supply-123-gm-0550-y1)	|ALT: Cooler Master V550 SFX Gold ($105)
TOTAL		|											|$834			|	|

<!-- Footer -->
&nbsp;

---

*This page was last updated on 2025-02-18*

