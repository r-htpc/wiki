# HDMI 2.0 Motherboards

<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
<style>
    table {
        width: 100%;
    }
</style>
-->

This is a list of motherboards that have or are suspected to have HDMI 2.0/HDCP 2.2 support.  

This can be via a HDMI 2.0, DisplayPort 1.2+ or a Thunderbolt 3 port. The latter two requiring a DP/TB->HDMI "active" adapter/cable for almost all TVs. If using a DP adapter, the specific list of motherboards can be ignored, but read the chipset notes; For DP 1.2, use [this](https://www.amazon.com/Monoprice-DisplayPort-1-2a-Active-Adapter/dp/B07FPQ4ZSW) adapter. For DP 1.4, use [this](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS), [this](https://www.amazon.com/CLUB-3D-CAC-1082-Active-Adapter/dp/B07HNTNTMR/ref=asc_df_B07HNTNTMR) or [this](https://www.amazon.com/Club-3D-DisplayPort1-4-Adapter-CAC-1085/dp/B08BX49V5V)  

**You don't have to look at this list for AMD Ryzen APUs or Intel >= 11th gen. HDMI 2.0 support is native and any motherboard is fine**

If you have one of these motherboards, or know someone that does, and is willing to test it, we'd be grateful.  

The only valid tests so far are: Playing Netflix 4K, Playing UHD blu-ray (SGX), [Cyberlink Advisor](https://www.cyberlink.com/prog/bd-support/diagnosis.do). All AMD RR+ boards should be able to support HDMI 2.0 (w/HDCP test on Picasso) but we only list boards here that are either user or vendor confirmed.  

&nbsp;

Here is the current motherboard list we've compiled, along with any sources as to their suspected or confirmed support. *"USERS"* refers to the results of user testing. *"YES"* means it is supported. *"NA"* means it hasn't been tested. *"VENDOR"* refers to what the mfgr says about support via specs/service.  *"SGX"* means it has been tested to play UHD blu-rays.  

Bolded boards are ones we recommend. Please read footnotes in () for specific qualifications and restrictions!  

&nbsp;

MOTHERBOARD|FORM|USERS|VENDOR|SOURCES/NOTES
---|---|---|---|---
AMD A3x0/B350/B450/X3x0/X470/X570|ALL|YES|YES|RR/PI Chipsets. All 2xxxG/3xxxG APUS
AMD A520/B550/X300/X570|ALL|YES|YES|RN/CZ Chipsets. All 4xxxG/5xxxG APUS
Intel Z490/H470/H410/B460|ALL|NA|YES|CML/RL Chipsets, ALL HDMI w/>= i5-11400 APUs (5b) or DP 1.2 w/[DP->HDMI adapter](https://www.amazon.com/Monoprice-DisplayPort-1-2a-Active-Adapter/dp/B07FPQ4ZSW) (6b). Otherwise only those with.. (5c)
Intel Z590/H570/H510/B560|ALL|NA|YES|CML/RL Chipsets, ALL HDMI w/>= i5-11400 APUs (5b). DP 1.2 w/[DP->HDMI adapter](https://www.amazon.com/Monoprice-DisplayPort-1-2a-Active-Adapter/dp/B07FPQ4ZSW) or DP 1.4, w/[USB-C->HDMI Adapter](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08MSWMXT4), [DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b). Otherwise only those with.. (5c)
Intel Z690/H670/H610/B660|ALL|NA|YES|ADL Chipsets, ALL HDMI w/12xxx, Gxxxx APUs or DP 1.4, w/[USB-C->HDMI Adapter](https://www.amazon.com/Cable-Matters-48Gbps-Adapter-Supporting/dp/B08MSWMXT4), [DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
EVGA H370 Stinger|M-ITX|YES (22a)|YES|CL, SGX, [specs](https://www.evga.com/products/product.aspx?pn=111-CS-E371-KR)
ASRock Fatal1ty Z170 Gaming-ITX/ac|M-ITX|YES (1a)|YES (1b)|SL/KL, SGX, MCDP2800 (19), [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](http://www.asrock.com/mb/Intel/Fatal1ty%20Z170%20Gaming-ITXac/?cat=Specifications)
ASRock Fatal1ty Z270 Gaming-ITX/ac|M-ITX|YES (2a)|YES (2b)|SL/KL, SGX, MCDP2800 (19), [Asrock HDCP 2.2 key DL](http://www.asrock.com/MB/Intel/Fatal1ty%20Z270%20Gaming-ITXac/index.asp#osW764), [Youtube review] (https://www.youtube.com/watch?v=Sztwg8FV5mk), [specs](http://www.asrock.com/MB/Intel/Fatal1ty%20Z270%20Gaming-ITXac/index.asp#Specification)
ASRock Fatal1ty Z370 Gaming-ITX/ac ($210)|M-ITX|YES (24a)|YES (24b)|CL, SGX, [specs](https://www.asrock.com/mb/Intel/Fatal1ty%20Z370%20Gaming-ITXac/#Specification)
ASRock Z390 Phantom Gaming-ITX/ac ($200)|M-ITX|YES (25a)|YES|CL/CL+, MCDP2800BC (19), [specs](https://www.asrock.com/mb/Intel/Z390%20Phantom%20Gaming-ITXac/index.asp#Specification)
ASRock Z490 Phantom Gaming-ITX/TB3|M-ITX|YES (25a)|YES (5b)|CML/CML+/RL, SGX, [specs](https://www.asrock.com/MB/Intel/Z490%20Phantom%20Gaming-ITXTB3/index.asp#Specification), HDMI 2.0 (5c), TB3, or DP 1.4 w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock Z490M-ITX/ac|M-ITX|NA|YES (5b,5d)|CML/CML+, [specs](https://www.asrock.com/mb/Intel/Z490M-ITXac/index.asp#Specification), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock H470M-ITX/ac|M-ITX|NA|YES (5b,5d)|CML/CML+, [specs](https://www.asrock.com/mb/Intel/H470M-ITXac/index.asp#Specification), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock B460M-ITX/ac|M-ITX|NA|YES|CML/CML+, [specs](https://www.asrock.com/MB/Intel/B460M-ITXac/index.asp#Specification), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock H410M-ITX/ac|M-ITX|NA|YES|CML/CML+, [specs](https://www.asrock.com/mb/Intel/H410M-ITXac/index.asp#Specification), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock H510M-ITX/ac ($110)|M-ITX|NA|YES|RL, [specs](https://www.asrock.com/MB/Intel/H510M-ITXac/index.asp#Specification), HDMI 2.0 (5d), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
ASRock Fatal1ty X370 Gaming-ITX/ac|M-ITX|YES (39a)|No (32b)|AMD RR/PI, [specs](https://www.asrock.com/mb/AMD/Fatal1ty%20X370%20Gaming-ITXac/#Specification)
ASRock Fatal1ty X470 Gaming-ITX/ac|M-ITX|NA|YES|AMD RR/PI/RN, [specs](https://www.asrock.com/mb/AMD/Fatal1ty%20X470%20Gaming-ITXac/index.asp#Specification)
ASRock X570 Phantom Gaming-ITX/TB3|M-ITX|NA|YES|AMD PI/RN, [specs](https://www.asrock.com/mb/AMD/X570%20Phantom%20Gaming-ITXTB3/index.asp#Specification)
ASRock Fatal1ty AB350 Gaming-ITX/ac|M-ITX|YES (40a)|No (32b)|AMD RR/PI, [specs](https://www.asrock.com/mb/AMD/Fatal1ty%20AB350%20Gaming-ITXac/index.asp#Specification)
ASRock Fatal1ty B450 Gaming-ITX/ac|M-ITX|NA|YES|AMD RR/PI/RN, [specs](https://www.asrock.com/mb/AMD/Fatal1ty%20B450%20Gaming-ITXac/index.asp#Specification)
ASRock B550M-ITX/ac ($130)|M-ITX|NA|YES|AMD RN/CZ, [specs](https://www.asrock.com/mb/AMD/B550M-ITXac/index.asp#Specification)
ASRock J3455-ITX ($80)|M-ITX|NA|YES|AL, MCDP2800-BC (19), [specs](http://asrock.com/mb/Intel/J3455-ITX/?cat=Specifications)
ASRock J4205-ITX|M-ITX|NA|YES|AL, MCDP2800-BC (19), [specs](http://asrock.com/mb/Intel/J4205-ITX/?cat=Specifications)
ASRock J4105-ITX ($100)|M-ITX|YES|YES|GL, [specs](http://asrock.com/mb/Intel/J4105-ITX/#Specification)
ASRock J5005-ITX|M-ITX|YES|YES|GL, [specs](http://asrock.com/mb/Intel/J5005-ITX/#Specification)
ASRock J4105M|M-ATX|YES|YES|GL, [specs](http://asrock.com/mb/Intel/J4105M/#Specification)
ASRock J4005M|M-ATX|YES|YES|GL, [specs](http://asrock.com/mb/Intel/J4005M/#Specification)
ASRock X570M Pro4|M-ATX|NA|YES|AMD PI/RN/CZ, [specs](https://www.asrock.com/mb/AMD/X570M%20Pro4/#Specification)
ASRock X570 Steel Legend|ATX|NA|YES|AMD PI/RN/CZ, [specs](https://www.asrock.com/mb/AMD/X570%20Steel%20Legend/#Specification)
ASRock X570 Creator|ATX|NA|YES|AMD PI/RN/CZ, [specs](https://www.asrock.com/mb/AMD/X570%20Creator/#Specification)
ASRock AB350M Pro4|M-ATX|YES (32a)|No (32b)|AMD RR/PI, [specs](https://www.asrock.com/mb/AMD/AB350M%20Pro4/index.asp#Specification)
Asus Prime B350M-A|M-ATX|YES (42a)|No (32b)|AMD RR/PI, [specs](https://www.asus.com/us/Motherboards/PRIME-B350M-A/specifications/)
Asus Prime B350M-E|M-ATX|YES (43a)|No (32b)|AMD RR/PI, [specs](https://www.asus.com/us/Motherboards/PRIME-B350M-E/specifications/)
Asus Z170-WS|ATX|NA|YES (3b)|SL/KL, MCDP2800 (19), [Overclockers review](http://www.overclockers.com/asus-z170-ws-motherboard-review/), [specs](https://www.asus.com/us/Motherboards/Z170-WS/specifications/)
Asus Z270-WS|ATX|YES (4a)|YES (4b)|SL/KL, SGX, [specs](https://www.asus.com/Motherboards/Z270-WS/specifications)
Asus Z170-DELUXE|ATX|NA|YES (3b)|SL/KL, SGX, [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](https://www.asus.com/us/Motherboards/Z170-DELUXE/specifications/)
Asus Z170-PREMIUM|ATX|NA|YES (3b)|SL/KL, SGX, [specs](https://www.asus.com/us/Motherboards/Z170-PREMIUM/specifications/)
Asus TUF B350M-PLUS GAMING|M-ATX|YES (46a)|No (32b)|AMD RR/PI, [avsforum](https://www.avsforum.com/forum/26-home-theater-computers/2980968-amd-2200ge-220ge-reasonable-htpc.html#post56279420), [specs](https://www.asus.com/us/Motherboards/TUF-B350M-PLUS-GAMING/specifications/)
Asus TUF B450M-PLUS GAMING|M-ATX|NA|YES|AMD RR/PI/RN, [specs](https://www.asus.com/us/Motherboards/TUF-B450M-PLUS-GAMING/specifications/)
Asus TUF B450M-PRO GAMING|M-ATX|NA|YES|AMD RR/PI/RN, [specs](https://www.asus.com/Motherboards/TUF-B450M-PRO-GAMING/specifications/)
Asus ROG STRIX B350-F GAMING|ATX|YES (41a)|No (32b)|AMD RR/PI, [specs](https://www.asus.com/us/Motherboards/ROG-STRIX-B350-F-GAMING/specifications/)
Asus ROG STRIX B450-I GAMING|M-ITX|NA|YES|AMD RR/PI/RN, [specs](https://www.asus.com/Motherboards/ROG-STRIX-B450-I-GAMING/specifications/)
Asus ROG STRIX X470-I GAMING|M-ITX|YES (49a)|YES|AMD RR/PI/RN, [specs](https://www.asus.com/us/Motherboards/ROG-STRIX-X470-I-GAMING/specifications/)
Asus ROG STRIX X570-I GAMING|M-ITX|NA|YES|AMD RR/PI/RN, [specs](https://www.asus.com/us/Motherboards/ROG-Strix-X570-I-Gaming/specifications/)
Asus ROG STRIX Z390-I GAMING ($230)|M-ITX|YES (7a)|YES|CL/CL+, SGX, ParadeTech PS175 (20), [specs](https://www.asus.com/us/Motherboards/ROG-STRIX-Z390-I-GAMING/specifications/)
**Asus Rog Strix Z490-I Gaming**|M-ITX|YES (25a)|YES (5b)|CML/RL, SGX, [specs](https://www.asus.com/Motherboards/ROG-STRIX-Z490-I-GAMING/specifications/), HDMI 2.0 (5c) or DP 1.4 w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
Asus Rog Strix B460-I Gaming|M-ITX|NA|MAYBE (5b)|CML, [specs](https://www.asus.com/Motherboards/ROG-STRIX-B460-I-GAMING/specifications/), no HDMI 2.0 port, DP 1.4 w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
Asus WS Z390 PRO ($400)|ATX|NA|YES|CL/CL+, [specs](https://www.asus.com/us/Commercial-Servers-Workstations/WS-Z390-PRO/specifications/)
Asus Prime Z490M-Plus|M-ATX|NA|NO (5b)|CML, [specs](https://www.asus.com/Motherboards/PRIME-Z490M-PLUS/specifications/), Says DP 1.4 but no 11th gen support, likely 1.2
GigaByte GA-Z170X-UD5 TH|ATX|NA|YES|SL/KL, MCDP2800 (19), [specs](http://www.gigabyte.com/Motherboard/GA-Z170X-UD5-TH-rev-10#ov)
GigaByte GA-Z170X-Gaming 7|ATX|NA|YES|SL/KL, MCDP2800 (19), [specs](http://www.gigabyte.com/Motherboard/GA-Z170X-Gaming-7-rev-10#ov)
GigaByte GA-Z170X-Gaming G1|E-ATX|NA|YES|SL/KL, MCDP2800 (19), [specs](http://www.gigabyte.com/Motherboard/GA-Z170X-Gaming-G1-rev-10#ov)
GigaByte GA-Z170X-Gaming GT|ATX|NA|YES|SL/KL, MCDP2800 (19), [specs](http://www.gigabyte.com/Motherboard/GA-Z170X-Gaming-GT-rev-10#ov)
GigaByte Aorus GA-Z270X-Gaming 8|ATX|YES (11a)|YES|SL/KL, SGX, MCDP2800 (19), [specs](http://www.gigabyte.com/Motherboard/GA-Z270X-Gaming-8-rev-10#kf)
GigaByte Aorus GA-Z270X-Gaming 9|E-ATX|YES (12a)|YES|SL/KL, SGX, MCDP2800 (19), [specs](http://www.gigabyte.us/Motherboard/GA-Z270X-Gaming-9-rev-10#kf)
GigaByte GA-X170-EXTREME ECC|ATX|NA|YES|SL/KL, MCDP2800 (19), C236 chipset, [specs](http://www.gigabyte.com/Motherboard/GA-X170-EXTREME-ECC-rev-10#ov)
GigaByte GA-A320M-S2H|M-ATX|YES (44a)|No (32b)|AMD RR, [specs](https://www.gigabyte.com/Motherboard/GA-A320M-S2H-rev-1x#sp)
**GigaByte B450 I AORUS PRO WIFI ($120)**|M-ITX|YES (47a)|YES|AMD RR, [specs](https://www.gigabyte.com/us/Motherboard/B450-I-AORUS-PRO-WIFI-rev-10#sp)
GigaByte B450 AORUS M|M-ATX|NA|YES|AMD RR, [specs](https://www.gigabyte.com/us/Motherboard/B450-AORUS-M-rev-10#sp)
GigaByte B450M DS3H|M-ATX|NA|YES|AMD RR, [specs](https://www.gigabyte.com/us/Motherboard/B450M-DS3H-rev-10#sp)
GigaByte GA-AB350M-DS3H|M-ATX|YES (45a)|No (32b)|AMD RR, [specs](https://www.gigabyte.com/Motherboard/GA-AB350M-DS3H-rev-1x#sp)
GigaByte GA-AB350N-Gaming WIFI|M-ITX|YES (41a)|No (32b)|AMD RR, [specs](https://www.gigabyte.com/us/Motherboard/GA-AB350N-Gaming-WIFI-rev-10#sp)
Gigabyte X570 I Aorus Pro Wi-Fi|M-ITX|NA|YES|AMD RR/PI/RN, [specs](https://www.gigabyte.com/us/Motherboard/X570-I-AORUS-PRO-WIFI-rev-10/sp#sp)
Gigabyte X570 UD|ATX|NA|YES|AMD RR+, [specs](https://www.gigabyte.com/us/Motherboard/X570-UD-rev-10/sp#sp)
**GigaByte Z390 I Aorus Pro Wi-Fi ($170)**|M-ITX|YES (25a)|YES|CL/CL+, SGX, [specs](https://www.gigabyte.com/us/Motherboard/Z390-I-AORUS-PRO-WIFI-rev-10#sp)
GigaByte Z370N-WIFI ($200)|M-ITX|YES (12a)|YES|CL, SGX, MCDP2800 (19), [specs](https://www.gigabyte.com/Motherboard/Z370N-WIFI-rev-10#sp)
GigaByte H370N-WIFI|M-ITX|YES (12a)|YES|CL, SGX, MCDP2800BC (19), [specs](https://www.gigabyte.com/Motherboard/H370N-WIFI-rev-10#sp)
Gigabyte Z490I Aorus Ultra|M-ITX|YES (26a)|YES (5b)|CML/RL, SGX, [specs](https://www.gigabyte.com/Motherboard/Z490I-AORUS-ULTRA-rev-10/sp#sp), HDMI 2.0 (5c) or DP 1.4 w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b). PS175 chip (20)
Gigabyte H470I AORUS Pro AX ($170)|M-ITX|YES (25a)|YES (5b)|CML/RL, SGX, [specs](https://www.gigabyte.com/Motherboard/H470I-AORUS-PRO-AX-rev-10/sp#sp), HDMI 2.0 (5c) or DP 1.4 w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b). PS175 chip (20)
GigaByte GA-IMB310TN|Thin M-ITX|YES (23a)|YES|CL, SGX, H310, [specs](https://www.gigabyte.com/Motherboard/GA-IMB310TN-rev-10#sp)
GigaByte GA-IMB370TN|Thin M-ITX|NA|YES|CL, Q370, [specs](https://www.gigabyte.com/Motherboard/GA-IMB370TN-rev-10#sp)
GigaByte J4005N D2P|M-ITX|NA|YES|GL, [specs](https://www.gigabyte.com/Motherboard/J4005N-D2P-rev-10#sp)
Supermicro C7Z270 PG|ATX|NA|YES|SL/KL, SGX, ParadeTech PS175 (20), [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](https://www.supermicro.com/products/motherboard/Core/Z270/C7Z270-PG.cfm)
Supermicro C7Z270 CG|ATX|YES (14a)|YES|SL/KL, SGX, ParadeTech PS175 (20), [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](https://www.supermicro.com/products/motherboard/Core/Z270/C7Z270-CG.cfm)
Supermicro C7Z370-CG-IW|M-ITX|NA|YES|CL, ParadeTech PS175 (20), [specs](http://www.supero.com/en/product-series/46-c7z370-cg-iw.html#product-features-tab-content)
Supermicro C9Z390-CG-IW|M-ITX|NA|YES|CL/CL+, SGX, ParadeTech PS175 (20), [specs](https://www.supermicro.com/products/motherboard/Core/Z390/C9Z390-CG-IW.cfm)
Supermicro C9Z390-PGW|ATX|NA|YES|CL/CL+, ParadeTech PS175 (20), [specs](https://www.supermicro.com/products/motherboard/Core/Z390/C9Z390-PGW.cfm)
Supermicro C9Z490-PGW / C9Z490-PG|ATX|NA|YES (5b)|CML/RL, SGX, ParadeTech PS175 (20), [specs](https://www.supermicro.com/en/products/motherboard/C9Z490-PGW). HDMI 2.0 (5c), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
Supermicro X11SAT-F|ATX|NA|YES|SL/KL, ParadeTech PS175 (20), C236 chipset, [specs](https://www.supermicro.com/products/motherboard/Xeon/C236_C232/X11SAT-F.cfm)
Biostar Z270GT9|ATX|YES (15a)|YES (15b)|SL/KL, SGX, MCDP2800-CC (19), [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](http://www.biostar.com.tw/app/en/mb/introduction.php?S_ID=861#specification)
Biostar Z270GT8|ATX|YES (16a)|YES (15b)|SL/KL, SGX, MCDP2800-CC (19), [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108), [specs](http://www.biostar.com.tw/app/en/mb/introduction.php?S_ID=860#specification)
Biostar Gaming Z170W|ATX|NA|YES (15b)|SL/KL, MCDP2800-BB (19), [specs](http://www.biostar.com.tw/app/en/mb/introduction.php?S_ID=806#specification)
Biostar Gaming Z170X|ATX|NA|YES (15b)|SL/KL, MCDP2800-BB (19), [Tweaktown review](http://www.tweaktown.com/reviews/7365/biostar-gaming-z170x-intel-z170-motherboard-review/index.html), [specs](http://www.biostar.com.tw/app/en/mb/introduction.php?S_ID=807#specification)
Biostar Racing X370GT5|ATX|YES (48a)|No (32b)|AMD RR, [specs](http://www.biostar-usa.com/app/en-us/mb/introduction.php?S_ID=873#specification)
Biostar Racing X370GT7|ATX|NA|YES (31b)|AMD RR, [specs](http://www.biostar.com.tw/app/en/mb/introduction.php?S_ID=874#specification)
Biostar Racing X570GT|M-ATX|NA|YES (31b)|AMD RR+, [specs](http://www.biostar-usa.com/app/en-us/mb/introduction.php?S_ID=957#specification)
Biostar Racing X570GT8|ATX|NA|YES (31b)|AMD RR+, [specs](http://www.biostar-usa.com/app/en-us/mb/introduction.php?S_ID=952#specification)
EVGA Z370 Classified K|ATX|YES (21a)|YES|CL, SGX, [specs](https://www.evga.com/articles/01151/evga-z370-series-motherboards/)
Colorful iGame Z370 Vulcan X V20|ATX|NA|MAYBE|CL, [specs](http://www.colorful.cn/product_show.aspx?mid=84&id=706#tabs-2)
MSI X370 XPOWER GAMING TITANIUM|ATX|NA|YES (33b)|AMD RR, [specs](https://www.msi.com/Motherboard/X370-XPOWER-GAMING-TITANIUM/Specification)
MSI B350I PRO AC|M-ITX|YES (41a)|No (32b)|AMD RR, [specs](https://www.msi.com/Motherboard/B350I-PRO-AC/Specification)
MSI B350M MORTAR|M-ATX|YES (41a)|No (32b)|AMD RR, [specs](https://www.msi.com/Motherboard/B350M-MORTAR/Specification)
MSI Meg Z490I Unify|M-ITX|NA|YES (5b,5d)|CML/RL, [specs](https://www.msi.com), DP 1.4, w/[DP->HDMI adapter](https://www.amazon.com/UPTab-DisplayPort-Adapter-displays-4096x2160/dp/B01B6ZOMIS) (6b)
IEI KINO-AQ170|M-ITX|NA|YES|SL/KL, Q170, [specs](https://www.ieiworld.com/en/product/model.php?II=431#specifications), HDMI 2.0, MCDP2800-BB (19)

&nbsp;

Intel Archs||||
:--|:--|:--|:--
AL=Apollo Lake|CL=Coffee Lake (8th Gen)|CL+=Coffee Lake Refresh (9th Gen)|CML=Comet Lake (10th Gen)
CML+=Comet Lake Refresh (10.5th Gen)|RL=Rocket Lake (11th Gen)|ADL=Alder Lake (12th Gen)|GL=Gemini Lake
KL=Kaby Lake (7th Gen)|SL=Sky Lake (6th Gen)||

AMD Archs||||
:--|:--|:--|:--
RR=Raven Ridge (2nd Gen)|PI=Picasso (3rd Gen)|RN=Renoir (4th Gen)|CZ=Cezanne (5th Gen)

SGX=Works with UHD blu-ray drives

&nbsp;

**EXAMPLE COMBINATIONS FOR 4K @ 60 Hz HDR**

* Intel: Config #1: i3-12100 ($125) + Any [H610/H670/B660 board](https://pcpartpicker.com/products/motherboard/) with HDMI ($100-120) = $225  

 *Micro-ATX: ASRock B660M-HDV ($95), Asus PRIME H610M-E D4 ($100)*  

* Intel: Config #2: i3-8100T/i5-8400T (ebay) ($100-$140) + ASUS TUF B365M-PLUS GAMING ($75) + [DP->HDMI cable](https://www.amazon.com/CLUB-3D-CAC-1082-Active-Adapter/dp/B07HNTNTMR) ($30) = $205-$245  

* Intel: Config #3: i3-10100 ($150) + Any [H410/H510/H470/B460/B560/Z490/Z590 board](https://pcpartpicker.com/products/motherboard/#xcx=0&f=7,8&c=144,149,141,142,151,150,143,148&sort=price) with Display Port ($100-$150) + [DP->HDMI cable](https://www.amazon.com/CLUB-3D-CAC-1082-Active-Adapter/dp/B07HNTNTMR) ($30) = $280-$330  

 *Micro-ATX: Asus PRIME B460M-A ($100), ITX: ASRock H510M-ITX/ac ($110)*  

* Intel: Config #4: i5-11400 ($190) + Any [H470\*/H510/H570/B560/Z490/Z590 board](https://pcpartpicker.com/products/motherboard/#xcx=0&f=7,8&c=149,142,151,150,143,148&sort=price) with HDMI ($100-$150) = $290-$340  

 *Micro-ATX: Asus PRIME B560M-A ($110), ITX: ASRock Z490 Phantom Gaming-ITX/TB3 ($200)*  

 \* *The cheapest H470 boards may not support 11th gen CPUs*  

* Intel: Config #5: i3-10100 ($150) + ASRock Z490 Phantom Gaming-ITX/TB3 ($200) = $350  

* AMD: Config #1: AMD 3200GE ($150) + A320 Motherboard with HDMI ($60-$100) = $210-$260  

* AMD: Config #2: AMD 3200G ($150) + B450 Motherboard with HDMI ($100-$150) = $250-$300  

 *Micro-ATX: Gigabyte B450 Aorus M ($90), ITX: GigaByte B450 I AORUS PRO WIFI ($140)*  

* AMD: Config #3: AMD 4350G ($190) + A520 Motherboard with HDMI ($75-$105) = $265-$295

* AMD: Config #4: AMD 4650G/5600G ($220) + B450/B550 Motherboard with HDMI ($100-$150) = $320-$370  

 *Micro-ATX: Gigabyte B550M DS3H ($95), ITX: ASRock B550M-ITX/ac ($130)*  

**EXAMPLE COMBINATIONS FOR 4K @ 120 Hz HDR**

* Intel: Config #1: i3-12100 ($125) + Any [H610/H670/B660/Z690 board](https://pcpartpicker.com/products/motherboard/) with Display Port 1.4 ($120) + [DP 1.4->HDMI 2.1 adapter](https://www.amazon.com/Club-3D-DisplayPort1-4-Adapter-CAC-1085/dp/B08BX49V5V) ($55) = $300  
  
* Intel: Config #2: i5-11400 ($200) + Any [H470*/H510/H570/B560/Z490/Z590 board](https://pcpartpicker.com/products/motherboard/#xcx=0&f=7,8&c=149,142,151,150,143,148&sort=price) with Display Port 1.4 ($100-$150) + [DP 1.4->HDMI 2.1 adapter](https://www.amazon.com/Club-3D-DisplayPort1-4-Adapter-CAC-1085/dp/B08BX49V5V) ($55) = $355-$405  

&nbsp;

FOOTNOTES  

(1a) [asrock forum](http://forum.asrock.com/forum_posts.asp?TID=4482&title=fatal1ty-z170-gamingitx-ac-uhd-bluray), /u/MemoryAlpha1

(1b) ASRock support

(2a) /u/taojoneses, [blu-ray forum](http://forum.blu-ray.com/showthread.php?t=287599&page=8) (2 users)

(2b) ASRock support

(3b) Asus support

(4a) User testing UHD blu-ray drive, [redfox forum](https://forum.redfox.bz/threads/new-in-powerdvd-17.72076/page-27)

(4b) Asus support, [asus specs](https://www.asus.com/Motherboards/Z270-WS/specifications)

(5b) DP 1.4 support contingent upon Intel 11th Gen Rocket Lake >= i5. Behavior on Comet Lake unknown.

(5c) HDMI 2.0 port is via LSPCON chip on motherboard so can use Comet Lake CPU.

(5d) HDMI 2.0 support contingent upon Intel 11th Gen Rocket Lake >= i5

(6b) For HDMI 2.1 support w/DP 1.4 use [Club3D CAC-1085 adapter](https://www.amazon.com/Club-3D-DisplayPort1-4-Adapter-CAC-1085/dp/B08BX49V5V). G-sync/Freesync is not supported over DP adapters

(7a) [blu-ray forum](https://forum.blu-ray.com/showpost.php?p=15843893&postcount=1156)

(11a) [blu-ray forum](http://forum.blu-ray.com/showthread.php?t=287599&page=7), [gigabyte forum](http://forum.gigabyte.us/thread/755/ga-z270x-gaming-8)

(12a) Pioneer, testing UHD blu-ray drives

(14a) /u/x820306, /u/imsoupercereal

(15a) BIOS to version Z27AF222 or later

(15b) Biostar support

(16a) BIOS to version Z27BF407 or later

(19) http://www.megachips.com/products/Data_Brief/MCDP28x0_Databrief.pdf

(20) https://www.paradetech.com/products/ps175/

(21a) UHD blu-ray playback [evga forum](https://forums.evga.com/4k-bluray-m2839216-p2.aspx)

(22a) UHD blu-ray playback [blu-ray forum](https://forum.blu-ray.com/showthread.php?p=15185625#post15185625)

(23a) UHD blu-ray playback, [blu-ray forum](https://forum.blu-ray.com/showpost.php?p=16460044&postcount=1199)

(24a) UHD blu-ray playback, [blu-ray forum](http://forum.blu-ray.com/showpost.php?p=13271422&postcount=108)

(25a) UHD blu-ray playback, [blu-ray forum](https://forum.blu-ray.com/showpost.php?p=16280880&postcount=1184)

(26a) UHD blu-ray playback, [blu-ray forum](https://forum.blu-ray.com/showpost.php?p=18850283&postcount=1345)

(24b) ASRock support

(31b) HDCP level unknown

(32a) /u/SommoLex

(32b) specs say no but AMD RR can do HDMI 2.0. HDCP level unknown.

(33b) HDCP level unknown. [msi datasheet](https://www.msi.com/pdf/presale/X370-XPOWER-GAMING-TITANIUM)

(39a) /u/dcpower89

(40a) [@coeusite SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(41a) [@Stefan75 SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(42a) [@kingeri SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(43a) [@gwilly7 SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(44a) [@atf SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(45a) [@Frung SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/)

(46a) [@willemd avsforum](https://www.avsforum.com/forum/26-home-theater-computers/2980968-amd-2200ge-220ge-reasonable-htpc.html#post56279420)

(47a) /u/Von_Satan (4k netflix), [@Legion SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/page-6#post-138331)

(48a) [@ooztuncer SFFForum](https://smallformfactor.net/forum/threads/raven-ridge-hdmi-2-0-compatibility-1st-gen-am4-motherboard-test-request-megathread.6709/page-6#post-138784)

(49a) [@benq999 Kodi Forum](https://forum.kodi.tv/showthread.php?tid=345566&pid=2885287#pid2885287)

&nbsp;

Let us know if any others should be added to the list.  

Obviously a board that lists the compatibility in its specs or any board that has a ParadeTech PS175/MegaChips MCDP2800 HDMI LSPCON chip is a candidate for HDMI 2.0.  

&nbsp;

We will be updating this table as we go.
