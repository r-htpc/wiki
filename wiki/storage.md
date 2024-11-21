# Storage Setup Guide

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

<!-- Section -->

## General

Spinning hard drives should be kept between 25C and 40C and temperature swings should be avoided where at all possible. Drives failure rates increase with heat, so do not pack more drives in a PC than you can effectively cool. SSDs should be kept below 70C to avoid performance throttling.  

If quick, no-delay access is required, APM/power management should be disabled so hard drives do not spin down and park their heads (see Disk Mgmt software below). 

Hard drive noise varies by vendor. Newer, helium-filled drives tend to be quieter than air-filled drives.

Recommended drives and related prices are given in the Hardware section below.  

<!-- Section -->

## Reliability

Different types of storage have different levels of reliability. The trick is to balance your needs with cost, space, and flexibility issues. Avoid "External Storage (USB/DAS)" and "Network Storage (Wifi)" where at all possible, but we will still provide solutions below. 

From Most reliable to Least reliable:

- Internal Storage (SATA/SAS)
- External Storage (PCIe SAS)
- Network Storage (LAN)
- External Storage (USB/DAS)
- Network Storage (Wifi)

<!-- Section -->

## Internal Storage

Large internal media storage usually consists of 3.5" HDD SATA drives, but also can be 2.5" SATA HDD drives if physical space is at a premium and <= 5TB of disk space is required. Markers of quality and general longevity are warranty, workload (TB/Yr), and M.T.B.F numbers.  
SSDs are good for smaller app, metadata and cache storage as they have more read/write performance and are quieter than HDDs. The value is not quite there for mass storage, so avoid for that use. 2.5" SATA SSD drives are good value for ephemeral space that doesn't need the best performance, while M.2 drives are better for higher IO performance and endurance.  

<!-- Section -->

## External Storage

External media storage can come in the format of USB drives or USB/Thunderbolt Direct Attached Storage enclosures (DAS); drives in a DAS can act as individual drives or as one drive. These USB-based storage devices are o.k. for beginner setups, but anything attached by **USB is at risk of being disconnected at random**, so **internal or network storage is preferred** to external, for reliability and stability. That said, if a DAS is PCIe SAS-based instead of USB, this is just as good as internal/network storage.  
**Never** do Software RAID or drive pooling over USB.  

Recommended DASes are bolded in the Hardware section below. PCIe solutions being preferred. 

Attach to a DiY or Ad-hoc solution below  

<!-- Section -->

## Network Storage

You should keep your network storage away from your listening environments/clients, both logically and physically, where at all possible. Logically because of it having a specialized OS different from front-ends makes it hard to combine tasks into a single system, Physically because of potential, combined noise and temperatures. Basements/media closets are ideal, but any space without drastic temperature fluctuations is fine.  

If you have the money to spend on a pre-built NAS and your requirements will not shift drastically, you should do that. Otherwise, looks at the other alternate options.  

<!-- Section -->

## Hardware

### Pre-Built NAS  
**(as of 2024-09-14)**  

The best option where cpu/mem requirements are not large and will not shift drastically. Becomes less cost effective as the number of drives increase, but may be justified if you really don't want to learn the ins/outs of DiY network storage and just want an easy, low-maintenance setup with a purpose-built pre-installed OS.  

There is a full list below, but the best pre-built NASes for the money are..  

If you just need storage..  
- 2 drives: Terramaster F2-212 - $170  
- 4 drives: Terramaster F4-212 - $230  

If you need storage and want to run backend services (like plex)..  
- 2 drives: Terramaster F2-423 - $280  
- 4 drives: Terramaster F4-424 - $500  

**STORAGE+SERVICES - 2 drives**  

BRAND		|	MODEL				|	DRIVES	|COST	|	TRANSCODING		|	CPU								|	PASSMARK	|	PM/$|	RAID MODES	| NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
**Terramaster**	|	**F2-423**				|	2	|	$280	|	4k (1a)	|	x64 (Celeron N5105) 2.0 Ghz	|		4094	|	14.6	|RAID 0/1,JBOD,Single|4GB RAM, 2.5 Gb/s
Terramaster	|	F2-424				|	2	|	$380	|	4k (1a)	|	x64 (Celeron N95) 3.4 Ghz	|		5419	|	14.26	|RAID 0/1,JBOD,Single|8GB RAM, 2x2.5 Gb/s
ASUSTOR		|	AS-5402T			|	2	|	$380	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094|	10.77	|RAID 0/1,JBOD,Single|4GB RAM, 2x2.5Gb/s, ext4/btrfs
Synology	|	DS224+				|	2	|	$300	|	Some/4k (1b)			|	x64 (Celeron J4125) 2.0 Ghz		|		3035	|	10.1	|RAID 0/1,JBOD,SHR,Single|2GB RAM, 1Gb/s x2
QNAP	|	TS-264				|	2	|	$425	|	4k (1a)			|	x64 (Celeron N5095) 2.0GHz		|		4125	|	9.7	|RAID 0/1,JBOD,Single|8GB RAM, 2.5Gb/s, ext4
Terramaster	|	F2-223				|	2	|	$260	|	Some/4k (1b)	|	x64 (Celeron N4505)	|		2241	|	8.62	|RAID 0/1,JBOD,Single|4GB RAM, 2x2.5 Gb/s

**STORAGE+SERVICES - 3+ drives**  

BRAND		|	MODEL				|	DRIVES	|COST	|	TRANSCODING		|	CPU								|	PASSMARK	|	PM/$|	RAID MODES	| NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
Terramaster	|	F4-424 Pro				|	4	|	$700	|	4k (0a)	|	x64 (i3-N305) 3.8 Ghz	|		10060	|	14.37	|RAID 0/1/5/6/10,JBOD,Single|ext4/btrfs, 32GB RAM, 2x2.5 Gb/s
**Terramaster**	|	**F4-424**				|	4	|	$500	|	4k (1a)	|	x64 (Celeron N95) 3.4 Ghz	|		5419	|	10.83	|RAID 0/1/5/6/10,JBOD,Single|ext4/btrfs, 8GB RAM, 2x2.5 Gb/s
**Terramaster**		|	**[F4-423](https://www.terra-master.com/us/f4-4607.html)**				|	4	|	$400	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094	|	 10.2	|RAID 0/1/5/6/10, JBOD, Single|ext4/btrfs, 4GB RAM , 2.5 Gb/s
QNAP		|	TS-364-4G				|	3	|	$450	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094	|	 9.09	|RAID 0/1/5,JBOD,Single|ext4, 4GB RAM, 2.5 Gb/s
Terramaster	|	[F6-424](https://www.terra-master.com/us/products/homesoho-nas/f6-424.html?page=menu&mid=1588)				|	6	|	$600	|	4k (1a)	|	x64 (Celeron N95) 3.4 Ghz	|		5419	|	9.03	|RAID 0/1/5/6/10,JBOD,Single|ext4/btrfs, 8GB RAM, 2x2.5 Gb/s
ASUSTOR		|	AS-5404T			|	4	|	$530	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094|	7.74	|RAID 0/1/5/6/10,JBOD,Single|4GB RAM, 2x2.5Gb/s, ext4/btrfs
QNAP		|	TS-464-4G				|	4	|	$550	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094	|	 7.44	|RAID 0/1/5/6/10, JBOD,Single|ext4, 4GB RAM, 2.5 Gb/s
Synology	|	DS423+				|	4	|	$500	|	Some/4k (1b)			|	x64 (Celeron J4125) 2.0 Ghz		|		3035	|	6.07	||2GB RAM
QNAP		|	TS-453D-4G				|	4	|	$500	|	Some/4k (1b)			|	x64 (Celeron J4125) 2.0 GHz		|		3035	|	6.07	|RAID 0/1/5/6/10,JBOD,Single|ext4, 4GB RAM
Terramaster		|	[T6-423](https://www.terra-master.com/global/products/smallmedium-businesses-nas/t6-423.html?page=menu&mid=1236)				|	6	|	$700	|	4k (1a)			|	x64 (Celeron N5105) 2.0 GHz		|		4094	|	 5.84	|RAID 0/1/5/6/10,JBOD,Single|ext4/btrfs, 4GB RAM (32)
Synology	|	DS1522+				|	5	|	$700	|	1080p			|	x64 (Ryzen R1600) 2.6 Ghz		|		3300|	4.71	||8GB RAM, 1 Gb/s x4

**JUST STORAGE - 2 drives**  

BRAND		|	MODEL				|	DRIVES	|COST	|	TRANSCODING		|	CPU								|	PASSMARK	|	PM/$|	RAID MODES	|	NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
**Terramaster**|	**[F2-212](https://www.terra-master.com/global/products/homesoho-nas/f2-212.html?page=menu&mid=1448)**				|	2	|	$170	|	Some 1080p/None	|	ARMv8.2 (Realtek 1619B) 1.7Ghz		|		NA		|	NA	|	RAID 0/1, TRAID, JBOD, Single	|	ext4/btrfs, 1GB RAM, 1 Gb/s
QNAP			|	TS-233				|	2	|	$200	|	Some 1080p/None	|	ARMv8.2 4-core 2.0Ghz		|		NA		|	NA	|	RAID 0/1, JBOD, Single	|	ext4, 2GB RAM, 1 Gb/s
Asustor			|	AS-1102T			|	2	|	$180	|	Some 1080p/None	|	ARMv8 (Realtek 1296) 1.4Ghz			|		NA		|	NA	|	RAID 0/1, JBOD, Single		|	ext4, 1GB RAM, 2.5 Gb/s
Synology		|	DS220j				|	2	|	$190	|	Some 1080p/None	|	ARMv8 (Realtek 1296) 1.4Ghz	|		NA		|NA|	SHR, RAID 0/1, JBOD, Single	|	ext4, 512MB RAM, 1 Gb/s

**JUST STORAGE - 4+ drives**  

BRAND		|	MODEL				|	DRIVES	|COST	|	TRANSCODING		|	CPU								|	PASSMARK	|	PM/$|	RAID MODES	|	NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
**Terramaster**		|	**[F4-212](https://www.terra-master.com/us/f4-212.html?page=menu&mid=1480)**				|	4	|	$230	|	Some 1080p/None	|	ARMv8.2 (Realtek 1619B) 1.7Ghz		|		NA		|	NA 	|	RAID 0/1/10/5/6, JBOD, TRAID, Single		|ext4/btrfs, 1/2GB RAM, 1 Gb/s
Asustor		|	1104T				|	4	|	$270	|	Some 1080p/None	|	ARMv8 (Realtek 1296) 1.4Ghz		|		NA		|	NA 	|	RAID 0/1/10/5/6, JBOD, Single		|ext4, 1GB RAM, 2.5 Gb/s
Terramaster	|	F5-221				|	5	|	$380	|	Some/4k 8-bit (3)	|	x64 (Celeron J3355) 2.0-2.5Ghz	|		1186	|	3.12	||

LEGEND  

Passmark = [CPU performance](https://www.cpubenchmark.net/cpu.php). Higher is better.  
PM/$ = Passmark per $. Higher is better.  
Transcoding = Plex transcoding ability, referenced in [plex's transcoding spreadsheet](https://docs.google.com/spreadsheets/d/1MfYoJkiwSqCXg8cm5-Ac4oOLPRtCkgUxU0jdj3tmMPc/edit#gid=1274624273)  
(0a) HW Transcoding: 3x 4k or 14x 1080p. SW Transcoding: 4x 1080p  
(1a) HW Transcoding: 2x 4k or 10x 1080p. SW Transcoding: 2x 1080p
(1b) HW Transcoding: 1x 4k or 4x 1080p. SW Transcoding: 1x 1080p + 1x 720p  
(2) HW Transcoding: 1x 4k or 3x 1080p. SW Transcoding: 1x 1080p  
(3) HW Transcoding: 2x 1080p. SW Transcoding: 2x 720p  
(4) HW Transcoding: 1x 1080p. SW Transcoding: 1x 720p  

### Ad-hoc  

If you can't afford a pre-built NAS and want to do it more cheaply, you can use/buy one of these and add external drives/enclosures to it:  

- Single Board Computer (SBC) or Pre-owned OEM PC

  - 1 drive: [NanoPi R2S](https://www.friendlyelec.com/index.php?route=product/product&path=69&product_id=282&sort=p.price&order=ASC) (USB2x1) $27, [Orange Pi Zero 3](https://www.aliexpress.us/w/wholesale-Orange-pi-zero-3.html?spm=a2g0o.productlist.search.0) (USB2x1) $25  

  - 2-4 drives:
    - USB-based: [Orange Pi 3 LTS](https://www.aliexpress.com/w/wholesale-orange-pi-3-lts.html) (USB3x1,USB2x2) $40, [RPI 4b](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/) (USB3x2,USB2x2) $35, [Rock64-2GB](https://ameridroid.com/collections/pine) (USB3x1,USB2x2) $35, [Pine H64](https://ameridroid.com/collections/pine) (USB3x1,USB2x2) $45, [Odroid C4](https://www.hardkernel.com/shop/odroid-c4/) (USB3x4) $55, PC: [Dell/Lenovo i3-4130t](https://www.ebay.com/sch/i.html?_from=R40&_nkw=%28i3-4130t%2Ci3-4160t%29&_sacat=171957&LH_TitleDesc=0&_sop=15&rt=nc) (USB3x2-4,USB2x2) $50. Optionally, add a [single enclosure DAS](/wiki/storage#direct-attach-storage-das-list) over USB.
    - SATA-based: [Odroid HC4](https://www.hardkernel.com/shop/odroid-hc4/) (**SATAx2**) $75, [Odroid H4+](https://www.hardkernel.com/shop/odroid-h4-plus/) + [Case](https://www.hardkernel.com/product-category/cases/) (**SATAx4**) $150.

  - Install linux or [Openmediavault](https://www.openmediavault.org/) as your OS, optionally create a storage pool under [mergerFS](https://github.com/trapexit/mergerfs/wiki) if more than one drive, and share your storage out [over the network with Samba](/wiki/storage#how-do-i-share-htpc-storage-on-my-network).  

- Wireless Access Point with USB port. if you already have one

  - Put it in AP mode on wired ethernet and [share the disk with samba](https://www.net-usb.com/share-hard-drive-over-network/#usb). Not advised for very large or non-powered drives. Get a SBC instead.  

### DiY   

If you want more CPU performance or more flexibility/expandability than any reasonably priced pre-built NAS or Ad-hoc solution can offer, build out your own DiY NAS with Unraid/TrueNAS/OMV and commodity hardware.  
Reference the DiY case/drive lists below, and the example builds under the [Wiki Sample Builds](/wiki/sample-builds#nasmedia-server-builds) page for full-part builds that range from used OEM pre-builts to ultimate DiY  

**If you want to skirt the line between a pre-built NAS and DiY, look at the following, as these can provide the same CPU/GPU performance as a pre-built NAS for cheaper, but give you more OS support with Windows, Linux or Unraid/TrueNAS/OMV compatibility and DiY-like flexibility:**  
- **Intel-based [Seeed Studio reServer (2 drives)](https://www.seeedstudio.com/reThings-reServer-c-2006.html)**  
- **Intel-based [AOOSTAR R1 (2 drives)](https://aoostar.com/products/aoostar-r1-2bay-nas-intel-n100-mini-pc-with-w11-pro-lpddr4-16gb-ram-512gb-ssd) / [AOOSTAR WTR PRO (4 drives)](https://aoostar.com/products/aoostar-n9e-intel-n100-mini-pc4c-4t-up-to-3-4ghz-with-w11-home-8-16gb-ddr4-3200mhz-ram-256-512gb-m-2-2280-nvme-ssd)**  

<!-- Sub-Section -->

### Direct Attach Storage (DAS)

As stated above, avoid USB based DASes. PCIe SAS is much more reliable. You can fit the low-profile PCIe cards into SFF sized servers (m920s) and even in a number of pre-built Micros (m920q/m90q, P320/P330 Tiny, ms-01).

<!--
Mediasonic	|	Proraid - HUR5	        |	2	|	$50		|	USB31G2, HW RAID 0/1, JBOD, Single
-->

BRAND		|	MODEL				|	DRIVES|	COST	|	NOTES
:--|:--|:--|:--|:--
Mediasonic	|	Probox - HF2/HF7	|	4	|	$100/$150	|	HF2: USB 3.0/eSATA, HF7: USB31G2
Mediasonic	|	Proraid - HFR2/HFR7     	|	4	|	$150/$180	|	USB30/USB31G2, HW RAID 0/1/10/3/5, JBOD, Single
Mediasonic	|	Probox - H82		|	8	|	$270-$350	|	USB30/USB31G2, Single
Terramaster       |       D4-300                     |      4       |       $170 | USB31G1, Single
OWC      |       [Mercury Elite Pro 2](https://www.amazon.com/OWC-Mercury-Elite-eSATA-Enclosure/dp/B06XRK93R9?th=1)  |      2       |       $65 | USB31G1/eSATA, Single
OWC      |       [Mercury Elite Pro Quad](https://www.amazon.com/OWC-Mercury-Elite-Storage-Enclosure/dp/B09SC124GS)  |      4       |       $220 | USB31G2, Single
**QNAP**		|	**[TL-D400S](https://www.qnapworks.com/TL-D400S.asp)**		|	4	|	$300	| **PCIe SAS (more reliable than USB)**, JBOD, Single
QNAP		|	TR-002-US		|	2	|	$160	| USB32G1, HW RAID 0/1/10/5, JBOD, Single
QNAP		|	TR-004-US		|	4	|	$200	| USB32G1, HW RAID 0/1/10/5, JBOD, Single
**PC Pitstop**           |       Various (Semi-DiY)  |    4-16    |  $350-1300   |  [Enclosure](https://www.pc-pitstop.com/sas-sata-enclosures-no-expander) + [PCIe SAS card](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=hba+%289201%2C9202%2C9207%29+%288e%2C16e%29&_sacat=56091&_odkw=hba+%288e%2C16e%29&_osacat=56091)
**Various**              |       Various (DiY)                    |       8-16   |       $250 | [PCIe SAS card](https://www.ebay.com/sch/56091/i.html?_from=R40&_nkw=%229202-16e%22)+[CASE](https://www.amazon.com/Cooler-Master-NSE-400-KKN2-Mid-Tower-Computer/dp/B00DKXXBU0)+[CAB1](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313&_nkw=8644+to+8644+cable+-sata+-8087+-8088+-8643+-8436&_sacat=58058&_odkw=8644+cable+-sata+-8087+-8088+-8643+-8436&_osacat=58058&_sop=15)+[ADAP](https://www.amazon.com/Adapter-Internal-SFF-8087-External-SFF-8088/dp/B01MFHET83?th=1)+[CAB2](https://www.ebay.com/sch/i.html?_from=R40&_nkw=8643+sata+cable&_sacat=58058&_odkw=8643+sata+cable&_osacat=58058)+[PSU](https://pcpartpicker.com/products/power-supply/#xcx=0&D=8,20&sort=price&page=1)+[FANS](https://www.amazon.com/Thermalright-TL-C12C-Computer-Included-Quantities%EF%BC%89/dp/B0BKKG1ZND)+[SPLIT](https://www.amazon.com/GELRHONR-Adapter-Cable%EF%BC%8C15-Splitter-Computer/dp/B09CGZQ2XF)
Various              |       Various (DiY)                    |       4      |       $125 | [PCIe SATA card](https://www.amazon.com/10Gtek-Profile-Bracket-Controller-Expansion/dp/B09Y1NRHX3)+[HDD Cage](https://www.google.com/search?q=rsv+sata+cage+34)+[Molex PSU](https://www.quietpcusa.com/Power-Supply/Power-Adapters-Converters-ACDC/Power-Adapter-110VAC-to-12VDC-w-4-pin-Molex-Connector-5-Amp)

<!-- Sub-Section -->

### Hard Drives

Recs bolded. Choose WD Ultrastar DC HC unless you need the lowest noise during read/write, then choose Ironwolf Pro NAS **NT** (you will give up cache size until 22TB model).  

BRAND					|CAPACITY|WARRANTY|INTERFACE|CACHE|WORKLOAD|Noise (1)|USE|NOTES		
:--|:--|:--|:--|:--|:--|:--|:--|:--
WD Elements/Easystore		|3-2TTB			|2 yr			|USB/SATA		|Various			|Various			|NA|USB, Shucked (pre-built or custom NAS)		|SMR, Cheapest
WD My Book				|3-2TTB			|3 yr			|USB/SATA		|Various			|Various			|NA|USB, Shucked (pre-built or custom NAS)		|SMR, Cheap
[Toshiba N300 NAS](https://www.toshiba-storage.com/wp-content/uploads/2017/08/TOSHIBA_16046_DS_N300_GB_Screen.pdf)			|4-18TB			|3 yr			|SATA			|128-256MB	|180TByr/1-1.2MHr	|20/NA|Pre-built or custom NAS					|CMR, 128MB <= 4TB, 256MB >= 6TB
[WD Red](https://documents.westerndigital.com/content/dam/doc-library/en_us/assets/public/western-digital/product/internal-drives/wd-red-hdd/product-brief-western-digital-wd-red-hdd.pdf)					|2-6TB			|3 yr			|SATA			|256MB		|180TByr/1MHr	|23/27|Pre-built or custom NAS					|SMR, 5.4K RPM
[WD Red Plus](https://documents.westerndigital.com/content/dam/doc-library/en_us/assets/public/western-digital/product/internal-drives/wd-red-plus-hdd/product-brief-western-digital-wd-red-plus-hdd.pdf)				|1-14TB			|3 yr			|SATA			|64-256MB	|180TByr/1MHr	|20/29|Pre-built or custom NAS					|CMR, 64MB <= 6TB, 256MB >= 8TB, 5.4-7.2K RPM
[WD Red Pro](https://documents.westerndigital.com/content/dam/doc-library/en_us/assets/public/western-digital/product/internal-drives/wd-red-pro-hdd/product-brief-western-digital-wd-red-pro-hdd.pdf)				|2-24TB			|5 yr			|SATA			|64-512MB	|550TByr/2-2.5MHr	|20/36|Pre-built or custom NAS					|CMR, 64MB <= 2TB, 256MB >= 4TB, 512MB >= 14TB
**[WD Ultrastar DC HC](https://www.westerndigital.com/products/data-center-storage/data-center-drives)**			|4-26TB			|**5 yr**			|SATA			|128-512MB	|**550TByr/2-2.5MHr**	|20/36|Pre-built or custom NAS					|CMR, 128MB <= 2TB, 256MB >= 4TB, **512MB >= 14TB**, [1-12TB](https://documents.westerndigital.com/content/dam/doc-library/en_us/assets/public/western-digital/collateral/cert/cert-ultrastar-sata-series-datasheet.pdf)/[14-18](https://documents.westerndigital.com/content/dam/doc-library/en_us/assets/public/western-digital/product/data-center-drives/ultrastar-dc-hc500-series/data-sheet-ultrastar-dc-hc550.pdf)
[Seagate Ironwolf NAS](https://www.seagate.com/content/dam/seagate/migrated-assets/www-content/datasheets/pdfs/ironwolf-18tb-DS1904-21-2207US-en_US.pdf)			|1-18TB			|3 yr			|SATA			|64-256MB	|180TByr/1MHr	|28/30|Pre-built or custom NAS					|CMR, 64MB <= 4TB, 256MB >= 6TB
[Seagate Ironwolf Pro NAS](https://www.seagate.com/products/nas-drives/ironwolf-pro-hard-drive/)		|2-24TB			|**5 yr**			|SATA			|128-512MB	|300-550TByr/1.2-**2.5MHr** (NE/**NT**)|**20/26 (NT)** 20/32 (NE)|Pre-built or custom NAS					|CMR, 128MB <= 4TB, 256MB >= 6TB, 512MB >= 24TB, [NT](https://media.flixcar.com/webp/synd-asset/Seagate-140535855-ironwolf-pro-20tb-DS2129-4-2311US-en_US.pdf)/[NE](https://www.seagate.com/files/www-content/datasheets/pdfs/ironwolf-pro-20tb-DS1914-19-2112US-en_US.pdf)
**[Seagate Exos X](https://www.seagate.com/products/enterprise-drives/exos-x/)**		|10-24TB			|**5 yr**			|SATA			|256-512MB	|**2.5MHr**	|28/32|Pre-built or custom NAS					|CMR, 256MB >= 10TB, 512MB (X24), [X16](https://www.seagate.com/files/www-content/datasheets/pdfs/exos-x16-DS2011-3-2008US-en_US.pdf)/[X18](https://www.seagate.com/files/www-content/datasheets/pdfs/exos-x18-channel-DS2045-3-2102US-en_US.pdf)/[X20](https://www.seagate.com/files/www-content/datasheets/pdfs/exos-x20-channel-DS2080-2111US-en_US.pdf)/[X24](https://www.seagate.com/content/dam/seagate/en/content-fragments/products/datasheets/exos-x24/exos-x24-DS2080-2307US-en_US.pdf)

(1) dBA for typical Idle/Seek operations on 12TB version (6TB for plain WD Red). Other models vary depending on family and air/helium filled.  

<!-- Sub-Section -->

### SSD Drives

Recs Bolded

BRAND 						|	SIZE | PCIE/INT | FORM | READ/WRITE | TBW  | CACHE	 | WARRANTY | USE | NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
Silicon Power A60				|	1TB		 | 3.0x4|	M.2 		|2200/1600	 | 600  | YES:SLC 	 | 5 yr 	 | CACHE | BEST $/GB, $60
**SK Hynix P31**				|	1TB		 | 3.0x4|	M.2 		|3500/3200	 | 750  | YES 		 | 5 yr 	 | STORE | $65
Samsung 970 Evo+			|	1TB		 | 3.0x4|	M.2 		|3500/3300	 | 600  | YES 		 | 5 yr 	 | STORE | $55
**Sabrent Rocket**					|	1TB		 | 4.0x4|	M.2 		|5000/4400	 | 1650 | YES 		 | 5 yr 	 | CACHE | BEST $/TBW, SB-ROCKET-NVMe4, $80
**SK Hynix P41**				|	1TB		 | 4.0x4|	M.2 		|7000/6500	 | 750  | YES 		 | 5 yr 	 | STORE | $90
**Kingston Fury Renegade**		|	1TB		 | 4.0x4|	M.2 		|7300/6000	 | 1000 | YES 		 | 5 yr 	 | STORE | $80
Sabrent Rocket 4+ 				|	1TB		 | 4.0x4|	M.2 		|7000/5400	 | 700  | YES 		 | 5 yr 	 | STORE | SB-RKT4P, $90
Samsung 980 Pro				|	1TB		 | 4.0x4|	M.2 		|7000/5000	 | 600  | YES 		 | 5 yr 	 | STORE | $60
WD SN850X					|	1TB		 | 4.0x4|	M.2 		|7300/6300	 | 600  | YES 		 | 5 yr 	 | STORE | $60
Samsung 990 Pro				|	1TB		 | 4.0x4|	M.2 		|7450/6900	 | 600  | YES 		 | 5 yr 	 | STORE | $90
Silicon Power A55				|	1TB		 | SATA|	M.2/2.5" 	|560/530		 | 500  | YES:SLC 	 | 3 yr 	 | CACHE | BEST $/GB, $35
Crucial MX500				|	1TB		 | SATA|	2.5"	 	|560/510		 | 360  | YES:1G 		 | 5 yr 	 | STORE | 1-4TB
**Samsung 870 Evo**			|	1TB		 | SATA|	2.5" 		|560/530		 | 600  | YES:1G 	 | 5 yr 	 | STORE | 1-4TB

TBW = Total Bytes Written, Workload

<!-- Sub-Section -->

### Hard Drive Prices (as of 2024-02-19)
Prices: [PCPartPicker](https://pcpartpicker.com/products/internal-hard-drive/#xcx=0&A=8000000000000,22000000000000&sort=price&page=1) (new). Recertified/refurbished/new pull prices are @20% less than new quoted below.  
Vendors: [Disctech](https://www.disctech.com), [Serverpartdeals](https://serverpartdeals.com), Amazon, Newegg 

BRAND						|8TB	|12TB	|14TB	|18TB
:--|:--|:--|:--|:--
WD Elements/Easystore		|$170	|$250 |$270 |$330
WD My Book					|$180	|$260 |$280 |$330
WD Ultrastar HC				|$170	|$275 |$240 |$350
Toshiba N300/Pro			|$150	|$250 |$285 |$330
WD Red Plus					|$190	|$230 |$355 |NA
WD Red Pro					|$230	|$290 |$300 |$340
Seagate Ironwolf NAS		|$170	|$200 |$240 |NA
Seagate Ironwolf Pro NAS	|$210	|$235 |$240 |$300
Seagate Exos X 				|$195	|$190 |$220 |$260

<!-- Sub-Section -->

### DiY NAS Case List

**For additional space to mount 3.5" HDDs, you can use:**  
PCI Slot to 3.5" HDD Adapter: [Micro connectors](https://www.amazon.com/dp/B07GDXBXPK/)  
5.25"x1 to 3.5"x1+2.5"x2 bay adapter: [Micro Connectors](https://www.amazon.com/dp/B07GDYNNWJ)  
5.25"x1 to 3.5"x1 bay adapter: [Metal 1-piece](https://www.amazon.com/dp/B07K8G41FZ), [Metal 2-piece](https://www.amazon.com/dp/B08YMMCXY2/), [Plastic](https://www.amazon.com/StarTech-com-3-5in-5-25in-Bracket-Adapter/dp/B000HLZXH2)  
5.25"x2 to 3.5"x3 bay adapter: [Evercool](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4)  
DiY drive cages: [2-drive](https://www.amazon.com/Phanteks-Stackable-Bracket-Cases-PH-HDDKT_03/dp/B07GY2B3WP), [5-drive](https://www.amazon.com/Sans-Digital-HDDRACK5-5-Bay-Organizing/dp/B001LF40KE), [10-drive](https://www.amazon.com/Kingjinglo-Stacking-Aluminum-Absorbing-Installation/dp/B09B9WCB3G)

CASE							|3.5"	|2.5"	|COST		|W x H x D (in)				|H.SWAP	|LITERS			|MOBOS				|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--
U-NAS NSC-201			|2		|1	|$130		|5.5 x 7.1 x 8				|**YES**	|6.4	|ITX				|w/150W Flex PSU. 47mm CPU. [link](https://www.u-nas.com/xcart/cart.php?target=category&category_id=249)
U-NAS NSC-401/410			|4		|2/3		|$150		|7.5 x 7.1 x 10				|**YES**	|8.7/10.1	|ITX				|w/250W Flex PSU. [link](https://www.u-nas.com/xcart/cart.php?target=category&category_id=249)
INNOVISION (U-NAS KNOCK-OFF)		|4		|NA		|$47-113+60	|7.4 x 7.1 x 10.3			|**YES**	|8.8			|ITX				|Shipping cost! 1U Flex PSU options - [link](https://www.aliexpress.com/item/4000151540264.html?spm=a2g0o.detail.1000060.2.3e9f65bd3NFIQG&gps-id=pcDetailBottomMoreThisSeller&scm=1007.14977.161853.0&scm_id=1007.14977.161853.0&scm-url=1007.14977.161853.0&pvid=28de11ce-d35d-40a4-bc22-7ac6928eb016&_t=gps-id:pcDetailBottomMoreThisSeller,scm-url:1007.14977.161853.0,pvid:28de11ce-d35d-40a4-bc22-7ac6928eb016,tpp_buckets:668%230%23131923%238_668%23808%235965%23588_668%23888%233325%233_668%232717%237558%23179)
Norco ITX-S4					|4		|NA		|$200		|7.75 x 7.5 x 10			|**YES**	|9.5			|ITX				|ITX-S8 version too
**Jonsbo N2**					|5		|1		|$150		|8.8 x 8.8 x 8.8			|**YES**	|11.1			|ITX				|65mm CPU, SFX PSU - [link](https://www.jonsbo.com/en/products/N2Black.html)
TOPLOONG NAS-6					|6		|NA		|$75+93		|10.23 x 7.67 x 9.84		|**YES**	|12.7			|ITX				|add +45 for 250W PSU - [link](https://www.aliexpress.com/item/4001316943062.html?spm=a2g0o.detail.1000014.5.5dd96f0c6YZrmJ&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.14976.195817.0&scm_id=1007.14976.195817.0&scm-url=1007.14976.195817.0&pvid=940ac58e-11f8-42df-89b7-d4eb52d1029a&_t=gps-id:pcDetailBottomMoreOtherSeller,scm-url:1007.14976.195817.0,pvid:940ac58e-11f8-42df-89b7-d4eb52d1029a,tpp_buckets:668%230%23131923%2379_668%23808%234094%23588_668%23888%233325%233_4976%230%23195817%236_4976%232711%237538%23641_4976%233104%239653%235_4976%234052%2318551%2393_4976%233141%239887%239_668%234328%2319924%23137_668%232846%238110%23377_668%232717%237558%23179_668%231000022185%231000066058%230_668%233422%2315392%237_4452%230%23194213%230_4452%233474%2315675%23168_4452%233098%239599%23462_4452%233564%2316062%23742)
Jonsbo N1					|5		|1		|$145		|6.69 x 8.54 x 13.93			|**YES**	|13.0			|ITX				|70mm CPU, SFX PSU - [link](https://www.jonsbo.com/en/products/N1.html)
**InWIN IW-MS04**					|4		|2		|$160		|8.3 x 9.10 x 10.80			|**YES**	|13.3			|ITX				|65mm CPU, 1U 265W-315W PSU, SFF-8087x1/8643x1/SATAx4 - [link](https://www.ipc.in-win.com/soho-smb-iw-ms04)
Supermicro CSE-721TQ-250B		|4		|NA		|$270		|8.27 x 9.45 x 11			|**YES**	|14.0			|ITX				|w/1U 250W Flex PSU
INNOVISION (UNAS KNOCK-OFF)		|6		|NA		|$83+76		|8.66 x 10.23 x 9.84		|**YES**	|14.3			|ITX				|Shipping cost! 1U Flex PSU - [link](https://www.aliexpress.com/item/4001180247506.html)
iStarUSA S-35-B4/B5/DE4/DE5				|4/5	|NA		|$140-160	|8.68 x 8.90 x 12.76		|**YES**	|16.2			|ITX				|1U Flex PSU
iStarUSA S-35-3/S-35EX			|3/5	|NA		|$85		|8.69 x 8.90 x 12.76		|No		|16.2			|ITX				|EX has 5.25"x3 (3.5"x5 with 5-in-3 adapter), 1U Flex PSU
Chenbro SR301					|4		|NA		|$240		|7.78 x 12.2" x 10.63		|**YES**	|16.5			|ITX				|SR30169. w/PSU
U-NAS NSC-810A				|8		|1		|$220		|12.4 x 7.8 x 10.8			|**YES**	|17.0			|uATX/ITX			|1x2.5 int, Flex PSU. [link](https://www.u-nas.com/xcart/cart.php?target=product&product_id=17640)
Norco ITX-S8					|8		|NA		|$230		|8 x 10.2 x 13.25			|**YES**	|17.7			|ITX				|1x2.5 int, SFF-8643x2, 1U Flex PSU. Hard to find
Jonsbo N3					|8		|1		|$155		|9.2 x 10.3 x 11.7			|**YES**	|18.2			|ITX				|130mm CPU, SFX PSU - [link](https://www.jonsbo.com/en/products/N3.html)
**Fractal Design Node 304**						|6		|NA		|$90		|10 x 8.27 x 14.72			|No		|19.3			|ITX/DTX			|165mm CPU, ATX PSU - [link](https://www.fractal-design.com/products/cases/node/node-304/black/)
Jonsbo N4					|8		|2		|$130		|11.3 x 9 x 11.8			|**YES**	|19.6			|uATX/ITX				|70mm CPU, SFX PSU - [link](https://www.jonsbo.com/en/products/N4Black.html)
FD Core 500						|3+1	|3		|$60		|9.84 x 8.39 x 14.96		|No		|20.2			|ITX/DTX			|ATX PSU, 1x5.25", +1 3.5" in 5.25" bay
Silverstone GD06				|4+1		|2		|$140		|17.32 x 5.91 x 13.39		|No		|22.4			|uATX/ITX			|70-120mm CPU COOL, ATX PSU, +1 3.5" in 5.25" bay, full dvd.
Silverstone DS380				|8		|4		|$215		|8.31 x 11.22 x 14.17		|**YES**	|21.6			|ITX				|SFX-L PSU, 57mm CPU.  [link](https://www.silverstonetek.com/en/product/info/server-nas/DS380/)
Raijintek Styx		|3		|4		|$70		|8.26 x 13.2 x 14.2	|No		|25.4			|uATX/ITX				|ATX PSU - [link](https://www.raijintek.com/en/products_detail.php?ProductID=26)
**Fractal Design Core 1000**		|2+2/3		|3		|$55		|6.89 x 13.97 x 16.53		|No		|26.1			|uATX/ITX/DTX				|2x5.25",2x3.5" - [link](https://www.fractal-design.com/products/cases/core/core-1000/black/)
Silverstone CS381				|8		|NA		|$400		|15.75 x 8.86 x 12.44 							|**YES**	|28				|uATX/ITX			|SFX-L PSU. [link](https://www.silverstonetek.com/en/product/info/server-nas/CS381/)
Silverstone PS16                |3+1        |3      |$75        |7.8 x 14.21 x 15.67        |No     |28.5           |uATX/DTX/ITX           |3x3.5",1x5.25"
**Silverstone TJ08-E**				|5+2/3		|NA		|$140		|8.27 x 14.72 x 15.16		|No		|30.2			|uATX/ITX/DTX		|5x3.5",2x5.25"
Silverstone GD08				|8+2/3		|2		|$180		|17.3 x 6.9 x 16.7			|No		|32.7			|EATX/ATX/uATX			|8x3.5",2x5.25", 138mm CPU COOL, ATX PSU. [link](https://www.silverstonetek.com/en/product/info/computer-chassis/GD08/)
Silverstone GD07				|5+4/6		|2		|$180		|17.3 x 6.9 x 17.1			|No		|33.5			|EATX/ATX/uATX			|5x3.5",4x5.25", 138mm CPU COOL, ATX PSU. [link](https://www.silverstonetek.com/en/product/info/computer-chassis/GD07/)
Cooler Master N200				|3+1		|4		|$55		|7.9 x 17.5 x 14.9 			|No		|33.7			|uATX/ITX				|3x3.5",1x5.25"
BitFenix Prodigy M 2022			|4	|5		|$100		|9.84 x 15.91 x 14.13		|No		|36.2			|uATX/ITX				|BFC-PM2-300-KKGSK-RP - [link](https://www.bitfenix.com/products/chassis/micro-atx/prodigy-m-2022/)
FD Focus G Mini					|2+2/3	|NA		|$55		|8.07 x 15.08 x 18.27		|No		|36.4			|uATX				|2x3.5",2x5.25", +2x3.5" in 5.25" (or +3 w/[Evercool adapter](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4)) Could probably fit 8x3.5 w/2x[Phanteks 2-drive](https://www.amazon.com/Phanteks-Stackable-Bracket-Cases-PH-HDDKT_03/dp/B07GY2B3WP) cages
Silverstone CS382				|8+1		|2		|$215		| 8.54 x 15.94 x 17.76							|**YES**	|39.6				|uATX/ITX			|1x5.25", 168mm CPU, ATX PSU. [link](https://www.silverstonetek.com/en/product/info/computer-chassis/cs382/)
**Cooler Master N300**           |8+2/3 |1      |$55        |7.5 x 19.4 x 16.8          |No     |39.8           |ATX/uATX           |8x3.5",2x5.25". [link](https://www.coolermaster.com/en-au/products/n300/)
**Cooler Master N400**	  	     |8+2/3	|3		|$80		|7.5 x 19.7 x 16.7			|No		|40.6			|ATX/uATX			|8x3.5",2x5.25". [link](https://www.coolermaster.com/catalog/cases/mid-tower/n400/)
**Fractal Design Node 804**		|8+2		|2/4		|$110			|13.5 x 12.0 x 15.3			|No		|40.3			|uATX/ITX			|ATX PSU, Cube - [link](https://www.fractal-design.com/products/cases/node/node-804/black/)
Silverstone CS380B				|8+2/3	|NA		|$190		|8.48 x 16.79 x 19.19		|**YES**	|44.7			|ATX/uATX/ITX			|ATX PSU, SATAx2 (12Gbps), 146mm CPU, 2x5.25"
Phanteks P400A			|2+4+2	|2		|$85		|8.3 x 18.5 x 18.3		|No		|46	|ATX/uATX/ITX		|2x3.5 (std)+4x3.5" (sleds)+2x3.5" (psu shroud top) 
Fractal Design Define R5			|8+2/3	|2		|$120		|9.1 x 17.7 x 20.5		|No		|47.3	|ATX/uATX/ITX		|8x3.5",2x5.25", +2x3.5" in 5.25" (+3 w/[Evercool adapter](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4)) + 2x3.5 on top (unofficially)? could fit 13 total?
Silverstone TJ04B-E				|9+4/6		|NA		|$245		|8.43 x 19.25 x 19.25		|No		|51.2			|CEB/ATX/uATX		|9x3.5",4x5.25"
Fractal Design Define 7		|13		|4		|$160		|9.4 x 18.7 x 21.5		|No		|57.7	|EATX/ATX/uATX/ITX		|13x3.5,1x5.25"
**Fractal Design Meshify 2**		|13		|4		|$140		|9.44 x 18.66 x 21.33	|No		|58.9	|EATX/ATX/uATX/ITX	|13x3.5 - [link](https://www.fractal-design.com/products/cases/meshify/meshify-2/black/)
Phanteks P500A			|10		|3		|$150		|9.5 in x 20.1 in x 20 in		|No		|61.8	|EATX/ATX/uATX/ITX		|2 HDD trays included - [link](https://phanteks.com/Eclipse-P500A.html)
Antec P101 Silent			|8+1		|2		|$125		|9.1 x 19.9 x 20.74 		|No		|61.8	|EATX/ATX/uATX/ITX		|8x3.5",1x5.25"
Fractal Design Define XL R2	|8+4/6	|NA		|$200		|9.1 x 22 x 22.04		|No		|70.2	|EATX/ATX/uATX/ITX		|8x3.5",4x5.25", +4x3.5" in 5.25" (+6 w/2x[Evercool adapter](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4))
Fractal Design Define 7 XL		|18		|5		|$210		|9.45 x 22.2 x 23.77		|No		|77.6	|EATX/ATX/uATX/ITX		|18x3.5"
Phanteks Enthoo Pro 2		|12		|NA		|$150		|9.45 x 22.8 x 22		|No		|78		|EATX/ATX/uATX/ITX	|4 HDD trays included

LEGEND  

Drives: xxx+yyy/zzz = 3.5" native+5.25" native/5.25" with adapter  
e.g. 4+2/3 = 3.5"x4 native + 3.5"x2 in 5.25"x2 bays (2 in 2) OR 3.5"x3 in 5.25"x2 bays w/[Evercool 5.25 adapter (3 in 2)](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4)  

<!-- Cheap, bad cable mgmt
DARKROCK Classico Storage Master	|10	|3		|$90		|8.07 x 18.5 x 16.92		|No	|41.4			|ATX/uATX/ITX			|ATX PSU, 4 fans inc, 160mm CPU. [link](https://darkflashtech.com/products/darkrock-classico-storage-master-case-atx-computer-case-mid-tower-with-4x120mm-fans-usb-3-0-ready-4-detachable-hard-drive-cages-360mm-supported-on-top-front-radiator-gpu-vertically-mounting-black)
-->

**DISCONTINUED CASES**

CASE							|3.5"	|2.5"	|COST		|W x H x D (in)				|H.SWAP	|LITERS			|MOBOS				|NOTES
:--|:--|:--|:--|:--|:--|:--|:--|:--
NAS6							|6		|NA		|$162		|8.43 x 8.5 x 11.65			|**YES**	|13.68			|ITX				|40mm CPU, 350W PSU included - [link](https://www.mini-itx.com/store/category?type=case)
Kolink Satellite Cube			|2/3		|2/4	|$49		|10.3 x 7.48 x 11			|NO		|13.8			|uATX/ITX				|165mm CPU, ATX PSU - [specs](https://kolink.eu/Home/case-1/mini-itx-2/satellite.html), [link](https://www.google.com/search?q=kolink+satellite+case)
HciPC 6bay P401-1 HCNAS			|6		|NA		|$65+70		|12.59 x 9.84 x 8.66		|No		|17.6			|ITX				|Node 304 clone. Pricey Shipping! - [link](https://www.aliexpress.com/item/32719919894.html?spm=a2g0o.detail.1000014.1.4bab14f6MEe7Us&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.14976.177813.0&scm_id=1007.14976.177813.0&scm-url=1007.14976.177813.0&pvid=b3e5fc96-0d9f-495e-b705-4d80981a3b5a&_t=gps-id:pcDetailBottomMoreOtherSeller,scm-url:1007.14976.177813.0,pvid:b3e5fc96-0d9f-495e-b705-4d80981a3b5a,tpp_buckets:668%230%23131923%2358_668%23808%235965%23588_668%23888%233325%233_4976%230%23177813%2316_4976%232711%237538%23700_4976%233223%2310328%232_4976%233104%239653%235_4976%233141%239887%239_668%232846%238110%23377_668%232717%237558%23179_)
Cooler Master Elite 120 Adv		|3+1	|NA		|Disc		|9.4 x 8.2 x 15.8			|No		|20				|ITX				|full dvd, 4x2.5 (from 2x3.5 bays), +1 3.5" in 5.25" bay
Cooler Master Elite 130		|2+1	|5		|$65		|9.4 x 8.2 x 15.7			|No		|20				|ITX				|full dvd, +1 3.5" in 5.25" bay
LIAN LI PC-Q25B					|5/7	|NA		|Disc		|7.83 x 11.02 x 14.41		|YES	|20.4			|ITX/DTX			|Hotswap (5) - Hard to find
Rosewill FBM-01/Ranger-M		|3+2/3	|0		|$35			|6.9 x 13.86 x 13.8/15.26			|No		|21.5/23.8			|uATX/ITX			|3x3.5",2x5.25", +2x3.5" in 5.25" (or +3 w/[Evercool adapter](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4))
Rosewill SRM-01B				|2+2/3		|2		|$35		|6.69 x 14.96 x 13.78		|No		|22.5			|uATX				|2x3.5",2x525", +2x3.5" in 5.25" (or +3 w/[Evercool adapter](https://www.amazon.com/EverCool-Dual-Drive-Triple-Cooling/dp/B0032UUGF4))
LIAN LI PC-M25					|5		|NA		|Disc			|7.83 x 12.67 x 17.36		|YES	|28.2			|uATX/ITX			|ATX PSU, 80mm CPU, +3.5x2 unofficial, 2.5x3 int, - Hard to find
Cooler Master Masterbox E300L	|2+2/3    	|NA		|$70		|7.1 x 14.33 x 17.6			|No		|29.3			|uATX				|2x3.5",2x5.25"
BitFenix Phenom					|5+1	|NA		|$90		|9.84 x 12.99 x 14.72		|NA		|30.8			|ITX				|BFC-PHE-300-	Hard to find
BitFenix Prodigy					|5+1	|NA		|$90		|9.84 x 15.91 x 14.13		|NA		|36.2			|ITX				|BFC-PRO-300- Hard to find
Lian-Li PC-V354					|7		|4		|Disc			|9.6 x 12.6 x 16.5			|No		|38.7			|uATX/ITX			|1x5.25, Cube
Lian-Li PC-V358				|6		|2		|Disc			|12.7 x 11.2 x 15.3			|No		|39.2			|uATX/ITX			|Cube
Fractal Design Core 1500		|4		|1		|Disc			|7.6 x 14.5 x 17.7			|No		|39.8			|uATX/ITX			|2x5.25
Lian Li PC-A05FN				|6		|NA		|Disc		|8.3 x 15.2 x 19.7			|NA		|40.7			|ATX				|NA
Lian-Li PC-A04					|7		|1		|Disc			|7.4 x 15.2 x 18.1			|No		|40.7			|uATX/ITX			|NA
Fractal Design Mini				|6+2/3		|0		|Disc			|8.2 x 15.5 x 19.2			|No		|42.9			|uATX/ITX			|2x5.25
Fractal Design Arc Mini R2		|6+2/3		|2		|Disc			|8.2 x 15.9 x 19.0			|No		|43.1			|uATX/ITX			|2x5.25
Lian-Li PC-08S				|6		|2		|Disc			|13.2 x 16.8 x 15.9		|No		|45.9	|EATX/ATX/uATX		|NA
Coolermaster NR600P		|6+2		|12		|Disc		|8.66 x 19.92 x 19.41		|YES		|54.9	|EATX/ATX/uATX/ITX		|2x Hot Swap - [link](https://www.coolermaster.com/catalog/cases/mid-tower/masterbox-nr600p/)

<!-- Section -->

## Software

If you're looking for a software storage solution for your DiY hardware, [Unraid](https://unraid.net) is highly suggested. If you can't afford it, then use  [Openmediavault](https://www.openmediavault.org/) with [mergerfs+snapraid](https://www.networkshinobi.com/snapraid-and-mergerfs-on-openmediavault/) or, if all disks will be the same size, RAID5 w/mdadm. If you need to use Windows, [StableBit DrivePool](https://stablebit.com/DrivePool) ($)+[snapraid](https://www.snapraid.it/). If you can't afford it, then Windows Storage Spaces.  

OS: [Unraid](https://unraid.net), [TrueNAS](https://www.truenas.com/truenas-scale/), [Openmediavault](https://www.openmediavault.org/), [Ubuntu Server](https://ubuntu.com/download/server), [Rockstor](http://rockstor.com)  

Software mgmt: Docker

Volume mgmt (windows): [Windows Storage Spaces](https://support.microsoft.com/en-us/windows/storage-spaces-in-windows-10-b6c8b540-b8d8-fb8a-e7ab-4a75ba11f9f2), [StableBit DrivePool](https://stablebit.com/DrivePool), [snapraid](https://www.snapraid.it/), [Elucidate (snapraid GUI)](https://github.com/Smurf-IV/Elucidate)  

Volume mgmt (linux): mdadm, [snapraid](https://www.snapraid.it/), [mergerFS](https://github.com/trapexit/mergerfs/wiki)  

Disk mgmt (windows): [CrystalDiskInfo](https://crystalmark.info/en/software/crystaldiskinfo/), [HDDScan](https://hddscan.com/), [WD Drive Utilities](https://support.wdc.com/downloads.aspx?DL=#WD_softwarepc)  

Disk mgmt (linux): smartctl, [hd-idle](http://hd-idle.sourceforge.net/)  

Benchmark (windows): [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/), [hdtune](https://www.hdtune.com/)  

Benchmark (linux): dd, hdparm  

<!-- Section -->

## Common Questions

<!-- Sub-Section -->

### How do I share HTPC storage on my network?

If your storage is on a linux-based OS, [follow these instructions](https://www.linuxbabe.com/ubuntu/install-samba-server-file-share) to use Samba  
If your storage is on a windows-based OS, [follow these instructions](https://support.microsoft.com/en-us/windows/file-sharing-over-a-network-in-windows-b58704b2-f53a-4b82-7bc1-80f9994725bf) to use Windows file sharing

<!-- Footer -->
&nbsp;

---

*This page was last updated on 2024-09-28*

