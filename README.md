# QuickstartSkyrimModdingGuide

###The Ultimate Skyrim Modding Guide

      
            ,        ,
            m   , ;  m
           ,m    k   m,      Ultimate
          ,mm   vm   mm,
         ,mmm  ` m   mmm,    Skyrim
        ,mmmm   m    mmmm,
       ,mmmmm, mmmm ,mmmmm,  Modding
      ,mmmmmmmmmmmmmmmmmmmm,
       ,mmmmm  mmmm  mmmmm,  Guide
        ,mmmm   mm   mmmm,
         ,mmm  mm    mmm,    /u/insane0hflex
          ,mm   m    mm,
           ,m    k,  m,      last updated 1/25/2016
            ,     `   ,
                 `
      

#Modding Skyrim Guide
Get started modding Skyrim with this quick and simple guide, perfect for those who are new to modding Skyrim or those returning from a long Skyrim hiatus.

###Laying the Foundation for Modding Skyrim
  - Buy the __Legendary__ version of Skyrim because it has all the DLCs. It's worth it. A lot of mods depend on resources from the DLCs.
  - Go to your Skyrim installation, usually located here: `C:\Program Files (x86)\Steam\steamapps\common\skyrim\`
  - Start up Skyrim with Steam
  - In Skyrim Launcher, choose the Ultra preset. Disable AA and FXAA if you plan to use an ENB
    - If you have older hardware or computer - set the Shadows to medium or high. 
      - Note: Shadows impact performance a lot. If needed, degrade the AA, Shadow, and/or resolution settings to gain more performance.
  - Start up Skyrim
  - Once you're at the main menu, exit the game
  - __ProTip__: You can quickly test out your performance by opening the console at the main menu by pressing the `~` key and typing `coc riverwood`
    - This command will create a level 1 character just outside Riverwood
    - You can test your performance in other locations by opening the console, then type `tmm 1` to unlock all map locations for fast travel.

- __Skyrim.ini__ changes
  - This file is usually located somewhere like:
    - C:\Users\YOUR_USER_NAME\Documents\My Games\Skyrim\
    - Put the changes underneath the ini section headers. 
    - Do not copy and paste in the section headers (ie: [General]), just copy the lines below it and before the next header
```
[General]
sIntroSequence=  ; disable the annoying intro video
fFlickeringLightDistance=4096 ; increases distance of visible light/torches

[Display]
fSunShadowUpdateTime=0.25 ; better sun shadow update time
fSunUpdateThreshold=1.5

[Combat]
f1PArrowTiltUpAngle=0.7 ; better bow reticle fixes
f3PArrowTiltUpAngle=0.7 ; vanilla bow settings are
f1PBoltTiltUpAngle=0.7  ; off true center by a bit
f3PBoltTiltUpAngle=0.7
```

- __SkyrimPref.ini__ changes
```
[Display]
...
iShadowMapResolution=2048 ; improves FPS without losing too much visual quality
...
bDrawLandShadows=1     ; Enable shadows that trees and land/rocks cast. 
bTreesReceiveShadows=1 ; Small performance hit, but increases graphical quality
...
bFloatingPointRender=1 ; Set this to 1 if you plan to use an ENB, otherwise leave this at 0
...
[Controls]
bMouseAcceleration=0   ; disables mouse acceleration
```

- Want to change your FOV? 
  - When Skyrim starts, at the main menu, press the `~` key to open the console
  - Type `fov ##` where ## is your desired FOV. I use 75 at 1080p.
  - Press the `Return/Enter` key to apply the FOV
  - When you restart Skyrim you should have the desired FOV setting applied.

- _Optional:_ At this point consider making a back up of your Skyrim folder, and your Skyrim.ini and SkyrimPref.ini files

###Install Skyrim Script Extender (SKSE)
  - Download: http://skse.silverlock.org
  - [SKSE Installation Tutorial video](http://www.youtube.com/watch?v=YfaJP-qT8z8)  
  - SKSE is required for a lot of mods to work, such as SkyUI, iHUD, and many more
  - From now on you will have to start Skyrim by using __skse_loader.exe__ (or by using the "SKSE" option in NMM or MO) to play Skyrim. If you don't, SKSE won't initialize to work in Skyrim.
  - Next, create a folder named `skse` in your `skyrim/data` folder
  - In here, create a new text file, and name it `skse.ini`
    - Next, put all of the following text inside `skse.ini`: 
```
[Display]
iTintTextureResolution=2048 ; more resolution to facepaints
[General]
ClearInvalidRegistrations=1 ; fixes orphaned scripts from mods
[Memory]
DefaultHeapInitialAllocMB=768 ; memory performance improvements
ScrapHeapSizeMB=256
```

###Create a Nexus Mods account
  - The [Skyrim Nexus](http://www.nexusmods.com/skyrim/) is where a large majority of mods are located
  - [Create Nexus Mod account](http://www.nexusmods.com/skyrim/users/register/)

###Install a Mod Manager
  - For simplicity and beginners:
    - [Nexus Mod Manager (NMM)](http://www.nexusmods.com/skyrim/mods/modmanager/)
  - For more control and advanced users:
    - [Mod Organizer (MO)](http://www.nexusmods.com/skyrim/mods/1334/)

###Install Load Order Optimisation Tool (LOOT)
  - Download: [LOOT](https://loot.github.io/)
  - Read the [LOOT documentation/readme](https://loot.github.io/docs/)

###Install the Unofficial Skyrim Patches
  - [Unofficial Skyrim Patch](http://www.nexusmods.com/skyrim/mods/19)
  - [Unofficial Dawnguard Patch](http://www.nexusmods.com/skyrim/mods/23491)
  - [Unofficial Hearthfire Patch](http://www.nexusmods.com/skyrim/mods/25127/)
  - [Unofficial Dragonborn Patch](http://www.nexusmods.com/skyrim/mods/31083/)
  - [Unofficial HD DLC Patch](http://www.nexusmods.com/skyrim/mods/31255/)
    - __Note:__ Only install this HD DLC patch if you use Bethesda's Official High Resolution DLC

###Install SkyUI
  - Download: [SkyUI](http://www.nexusmods.com/skyrim/mods/3863)
  - Provides a superior user interface experience
  - SkyUI also has "Mod Configuration Menu (MCM)" - which is used by many other mods to configure options/settings
  
###Install iHUD
  - Download: [iHUD](http://www.nexusmods.com/skyrim/mods/3222)
  - iHUD "hides the HUD when not needed, shows the HUD when it is needed"

###Install Enhanced Camera
  - Download: [Enhanced Camera](http://www.nexusmods.com/skyrim/mods/57859)
  - Enables a real first person view - now you can see your body in first person!

###Now research and install mods that interest you.
  - You __must__ read the mod description of every mod you download.
  - Carefully read the Compatibilty section of a mod's description.
  - Some mods require patches with other mods.
  - Run LOOT after installing mods to sort your load order so your game doesn't crash
    
###Discover Skyrim Mods from these Skyrim Mod Related YouTubers
  - [Gopher](http://www.youtube.com/gophersvids)
  - [insane0hflex](http://www.youtube.com/insane0hflex)
  - [Brodual](http://www.youtube.com/brodual)
  - [Hodilton](http://www.youtube.com/hodilton)

###Essential Mods
These mods improve Skyrim without altering gameplay mechanics.
- __UI__
  - [moreHUD](http://www.nexusmods.com/skyrim/mods/51956/?)
  - [Even Better Quest Objectives](http://www.nexusmods.com/skyrim/mods/32695)
  - [A Quality World Map with Roads](http://www.nexusmods.com/skyrim/mods/4929)
  - [No Menu and Loading Screen Smoke](http://www.nexusmods.com/skyrim/mods/7901/?)

- __Textures__
  - [Enhanced Blood Textures](http://www.nexusmods.com/skyrim/mods/60)
  - [Book Covers](http://www.nexusmods.com/skyrim/mods/35399)
  - [Enhanced Distant Terrain v2](http://www.nexusmods.com/skyrim/mods/39394)
  - [Static Mesh Improvement Mod](http://www.nexusmods.com/skyrim/mods/8655)
  - [Superior HD Hair Textures](http://www.nexusmods.com/skyrim/mods/36510/?)
  - [Xenius HD Character Textures](http://www.nexusmods.com/skyrim/mods/2356/?)

- __Realism/Immersion__
  - [Wet and Cold](http://www.nexusmods.com/skyrim/mods/27563/)
  - [Interesting NPCs](http://www.nexusmods.com/skyrim/mods/8429)
  - [Open Faced Guard Helmets](http://www.nexusmods.com/skyrim/mods/9514/?)
  - [Realistic Ragdolls and Force](http://www.nexusmods.com/skyrim/mods/601/?)


###Troubleshooting
  - If you get a CTD on loading into a save, usually a mod is causing the problem.
  - WIP ... 

-----

#TLDR Guide to Modding Skyrim
  - Buy and install [Skyrim: Legendary Edition](http://store.steampowered.com/sub/28187/) - You want the Legendary edition for all the DLC. Lots of mods require all the DLCs and the DLCs themselves are good (except for Hearthfire, but a lot of mods use that DLC's assets)
  - Install [Skyrim Script Extender SKSE](http://skse.silverlock.org/)
    - [SKSE Installation Tutorial video](http://www.youtube.com/watch?v=YfaJP-qT8z8)
  - Install [LOOT](https://loot.github.io/)
    - Read the LOOT readme/documentation to get an idea on how to use LOOT
  - Create a [Nexus Mod account](http://www.nexusmods.com/skyrim/users/register/) - to download mods from the [Skyrim Nexus](http://www.nexusmods.com/skyrim/)
  - Install a Mod Manager
    - Pick one: 
      - [Nexus Mod Manager (NMM)](www.nexusmods.com/skyrim/mods/modmanager/) - Very Beginner friendly
      - [Mod Organizer (MO)](www.nexusmods.com/skyrim/mods/1334/) - Advanced features and better than NMM but takes time to learn and set up
  - Install [SkyUI](http://www.nexusmods.com/skyrim/mods/3863) 
  - Install [iHUD](http://www.nexusmods.com/skyrim/mods/3222)
  - Install [EnhancedCamera](http://www.nexusmods.com/skyrim/mods/57859)
  - Install the Unofficial Skyrim Patches
    - [Unofficial Skyrim Patch](http://www.nexusmods.com/skyrim/mods/19)
    - [Unofficial Dawnguard Patch](http://www.nexusmods.com/skyrim/mods/23491)
    - [Unofficial Hearthfire Patch](http://www.nexusmods.com/skyrim/mods/25127/)
    - [Unofficial Dragonborn Patch](http://www.nexusmods.com/skyrim/mods/31083/)
    - [Unofficial HD DLC Patch](http://www.nexusmods.com/skyrim/mods/31255/) __Note:__ Only install this HD DLC patch if you use Bethesda's Official High Resolution DLC
  - Sort your mod load order using LOOT
  - Discover more mods by browsing the Nexus or check out My "Essential" mod list:
    
  
