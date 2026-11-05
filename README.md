## LATEST NEWS:
* ### New SWTOR IO Tools Blender add-on. Test the Beta release!
  **[SWTOR IO Tools](https://github.com/UnconventionalError/SWTOR-Import-Export-Tools/releases)** is a new Blender add-on that puts under a single umbrella vastly improved versions of our tools. We expect it to replace both **Darth Atroxa's** [**.gr2 importer add-on**](https://github.com/SWTOR-Slicers/Granny2-Plug-In-Blender-2.8x) and separate tools like the [**ZG SWTOR Tools**](https://github.com/SWTOR-Slicers/ZG-SWTOR-Tools)' **Area and Character Assemblers**.

  This new add-on provides:
  * Improved .gr2 object and skeletons import.
  * **Cloth physics!**
  * **64 bit animations!**
  * Conventional SWTOR materials (no custom panels, .blend template file-based for easy maintenance) that are far easier to modify and customize. Smart to conventional materials converter. The old smart materials are still available. New supported materials!
  * **Character Assembler** that grabs the assets directly from a game asset extraction. 
  * **Area Assembler** that imports and textures terrain patches, scatters objects (grass, rocks, etc.), and many other improvements.
  * fxspec-defined objects import (decorations, etc.).
  * Etc.

    (.gr2 export for modding isn't tested yet, specially because it intends to support attachments)

  **Fellow Slicer Crunch (AKA [UnconventionalError](https://github.com/UnconventionalError)) has been working on this for months**, with help from Jedipedia.net developer **C-3PO**, contributions by **Captn. Koda**, and others. We hope to be able to deprecate the older tools (which we'll keep around for those who still need them: people who have built their own tools around them, modders, and those that can't run Blender 4.5 and higher), and create new ones around this add-on.

  You can download the latest versions [here](https://github.com/UnconventionalError/SWTOR-Import-Export-Tools/releases). It can coexist with the .gr2 Importer and with the ZG Tools in a same Blender installation, but only one of the two sets can be enabled at once to avoid issues. Please disregard the new add-on's ReadMe, as for now it is a copy of the original one and needs a full rewrite.

* ### About TORCommunity.com and its Character Designer.
  Its owner transplanted the site to a new server, so, TORC is now downraight zippy 🙂. BUT:
  * **The Character Designer didn't survive the move**.
  * **The site's data is still stuck in Game Update 7 or older**.

  The NPC database's exporters still work, but at this moment it's better to use Jedipedia.net's ones: they are up-to-date and compatible with both the ZG SWTOR Tools' Character Assembler and the new SWTOR IO Tools' one.

  There is hope that TORC can eventually be updated, but it would involve a considerable amount of work. So, for the time being and the foreseeable future, we must live without its Character Designer. There are some means to reproduce its functionality through other tools, and then there's the old manual approach.
  
* ### About this Wiki.
  Obviously, given these news and previous developments, **there are whole chunks of this wiki that are no longer actionable, especially all the stuff related to automatic Player Character assembling**, and also we are lacking in guides on modding and porting (there is a ton of activity in our Discord regarding those, but very little has translated to guides). Hopefully we'll be able to do something about it once the dust settles.


# Welcome to the SWTOR Slicers wiki!


We are a group of swtor fans who enjoy messing with the game and pulling out models, textures, etc. This GitHub repository contains tools and guides to help you do so yourself, as well as some other things.

In this Wiki we pool all the knowledge we are gathering on SWTOR's data and how to use it, be it to discover what Broadsword is cooking (datamining), to enhance our SWTOR experience by changing the game's looks (modding, sadly on hiatus at the moment as the tools need upgrading), or to make art out of the game's assets and immortalize our player characters through other 3D apps or even 3D-printing (extracting). Bear with us: it's far easier than it looks 🙂.

We encourage you to join our [**SWTOR Slicers Discord Server**](https://discord.gg/XfHFjSN), where you will be able to interact with fellow hobbyists in a direct manner, find help if you get stuck, and even contribute if you feel like it.

(You can find a few of us in the popular **SWTOR Artists Discord Server**'s 3d art channels, too)

***
(We do not condone the usage of our tools for malicious intent, including: **exploits**, **harassment of others**, or anything else that may violate EA/Bioware's [EULA](https://www.swtor.com/legalnotices/euala), [TOS](http://www.swtor.com/legalnotices/termsofservice), [DSA](https://www.swtor.com/legalnotices/digitalservicesagreement), [Privacy Policy](https://www.swtor.com/legalnotices/privacypolicy) Copyrights, Trademarks, or anything else illegal. We will not be held accountable for your actions, and will act against you if it becomes necessary)

***
* [Home.](https://github.com/SWTOR-Slicers/WikiPedia/wiki)
* **[State of Play November 2026](https://github.com/SWTOR-Slicers/WikiPedia/wiki/state-of-play)**
* Getting Help:
  * [Link to the SWTOR Slicers Discord Server.](https://discord.gg/XfHFjSN)
  * [TORCommunity and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)
  * [Jedipedia and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)

***

### INTRODUCTION

 [**IMPORTING SWTOR MODELS INTO BLENDER: A BRIEF OVERVIEW**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-SWTOR-models-into-Blender-An-overview)  
  **Check this intro first. Afterwards, you can jump directly to the guides on extracting PCs, NPCs and others**. 

***

### DOWNLOADABLE TOOLS:

* **ExtracTOR (Windows app)**: extracts the game assets from SWTOR's files.  
  **[Download](https://github.com/UltimaKaosXIII/extracTOR/releases/latest)** - **[Guides](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ExtracTOR)**.
  
* **Blender (Windows/macOS/Linux app)**: popular free, open source 3D app.  
  **[Download](https://www.blender.org/download/lts/)** - **[Guides](https://www.blender.org/support/)** - **[Short videoguides](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)**


* **.gr2 Import/Export Add-on for Blender**: imports 3D models in SWTOR's .gr2 format.  
  **[Download .gr2 and ZG Add-ons](https://github.com/SWTOR-Slicers/ZG-SWTOR-Tools/releases/latest)** - **[Guides](https://github.com/SWTOR-Slicers/Granny2-Plug-In-Blender-2.8x#swtor-granny2-gr2-importexport-add-on-for-blender-28-to-42)**.

* **ZG SWTOR Tools Add-on for Blender**: includes Character and Area Assemblers.  
  **[Download .gr2 and ZG Add-ons](https://github.com/SWTOR-Slicers/ZG-SWTOR-Tools/releases/latest)** - **[Guides](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ZG-SWTOR-Tools-Add-on)**.

* **SWTOR Terrain Extractor (Windows command line executable)**: pre-converts SWTOR's ground patches files to a format (.obj) readable by our tools:    
  **[Download](https://github.com/UltimaKaosXIII/STE2/releases/latest)** - **[Guides](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-Terrain-Extractor)**.

* **JC SWTOR Tools Add-on** for [Blender 3.6 LTS](https://www.blender.org/download/lts/3-6/) only:  
  Character, Gear, Dye, and NPC importer that doesn't use TORCommunity.com data:  
  **[Download](https://github.com/jecandone/JC-SWTOR-Tools/releases/latest)** - **[User Guides](https://github.com/jecandone/JC-SWTOR-Tools)**  
  **[Requires installing matched .gr2 and ZG add-ons, too](https://github.com/SWTOR-Slicers/ZG-SWTOR-Tools/releases/latest)**.

(Older tools like Slicers GUI, Noesis, or EasyMYP, are no longer needed, supported, or compatible at all)




### ONLINE TOOLS:

  * **[TORCommunity.com](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)**:  
  (warning: it runs VERY slowly)
    * [SWTOR Database](https://torcommunity.com/database/search/all) (with NPC Exporters).
    * [Character Designer](https://torcommunity.com/tools/character-designer).

  * **[Jedipedia.net](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)**:
    * [SWTOR Database](https://swtor.jedipedia.net/en).
    * [File Reader](https://swtor.jedipedia.net/reader) ([provisional guide](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Jedipedia-File-Reader)).
    * [World Viewer](https://swtor.jedipedia.net/viewer).
  


***

### THE COMPLETE GUIDE TO AUTO-EXTRACTING AND ASSEMBLING PLAYER CHARACTERS AND NPCs:

**[READ THE BROAD STROKES FIRST: YOU'LL SEE IT'S EASIER THAN YOU THINK!](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically)**
  * The steps:
    * [Extracting SWTOR's game assets with ExtracTOR (WIP).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Installing-ExtracTOR-and-extracting-the-game-assets)
    * [Using TORCommunity's Character Designer to export Player Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-Character-Designer)
      * **IF ARMOR SELECTION SEARCH IS DOWN:** [workaround to manually specify Armor Sets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORC-Character-Designer-and-Manually-Creating-Armor-Sets)
    * [Using TORCommunity's NPCs Database to export Non Playable Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-NPCs-Database)
    * [Using our Blender add-ons to auto-assemble the model.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-the-character-with-the-Character-Assembler-Tool)
    * [Rigging the character for posing and animation](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Binding-a-character-to-a-posing-skeleton)
    * [Applying SWTOR animations to the character.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Applying-SWTOR-animations-to-a-skeleton)  

* Extra steps that require manual work and some knowledge of SWTOR's assets:
    * [Making capes and hair work, manually and through Cloth Simulation.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Making-capes-and-hair-work,-manually-and-through-Cloth-Simulation)
    * [Making Twi'lek lekku work for poses and animations.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Rigging-Twilek-Lekku-for-Poses-and-Animation)
    * [Locating weapons' assets manually.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
    * [Attaching weapons and other objects to a character **with a SWTOR rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character)
    * [Attaching weapons and other objects to a character **with a custom rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character-with-custom-rigs)
  
### Baking the models' textures and exporting to other apps:
  * Baking:
    * [Converting SWTOR materials to baking-friendly ones.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-models-to-export-them-to-other-apps)
    * [Baking an object's multiple materials into a single one.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-multiple-materials-of-an-object-into-a-single-one)
  * Exporting to other apps:
    * [Exporting to VRChat.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-SWTOR-models-to-VRChat)
    * [Exporting to Star Wars Battlefront II.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-SWTOR-models-to-Battlefront-II)
    * Exporting to Unreal Engine.
    * [Exporting to Garry's Mod](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-to-Garrys-Mod-(GMod)).
    * Exporting to Tabletop Simulator.
  * 3D Printing:
    * [Baking Normals into real 3D detailing](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-Normals)

***

### ASSEMBLING GAME LOCATIONS AUTOMATICALLY:

* [Assembling SWTOR Game Areas with Jedipedia.net data and ZG SWTOR Tools Add-on's Area Assembler](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ZG-SWTOR-Area-Tools).

***

### LOCATING AND ASSEMBLING ASSETS MANUALLY:

* [**Locating Player Characters' head assets through their Appearance Designer sliders data**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Understanding-In-Game-Head-Slider-Values)
* [**Locating armor parts' assets**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-Armor-Parts-Assets)
* [Locating weapons' assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
* [Assigning materials and textures to environmental and architectural elements, furniture, props, ships, vehicles and weapons.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assigning-materials-and-textures-to-environmental-and-architectural-elements,-furniture,-props,-ships,-vehicles-and-weapons)
* [Assembling multi-part assets (Decorations, Rooms, etc).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assembling-Multi-Part-Assets-(Decorations,-Rooms,-etc))
* [Generic guide to importing objects and assigning materials (**Legacy Add-on-based**. Needs updating).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-Objects-and-Assigning-Materials-in-Blender)

***

### OTHER GUIDES (WIP):

  * [Snippets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Snippets)
  * Improving and customizing our SWTOR models and materials.
    * [List of tips and tricks to cover in the future.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Blender-and-SWTOR-Tips-and-Tricks)
    * [Replacing body parts with gear vs. putting gear on top of body parts](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Replacing-body-parts-with-gear-vs.-putting-gear-on-top-of-body-parts)
    * [Merge by Distance before applying Modifiers.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Merge-by-Distance-before-applying-Modifiers)
    * [Enhancing SWTOR texture maps with Cupscale.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Enhancing-SWTOR-texture-maps-with-Cupscale)
  * [Other Extracting Strategies (needs updating).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-strategies)
  * SWTOR Materials recipes:
    * [SWTOR’s holosigns: how to make them work in Blender.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-holographic-signs-and-how-to-make-them-work)

***

### MODDING
**We have resumed modding tool development. Stay tuned for tools and tutorials.  
Meanwhile, visit [our Discord](https://discord.gg/XfHFjSN)'s Modding channel**
* Alternative techniques:
  * [Modding SWTOR textures with Special K](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Modding-SWTOR-textures-with-Special-K) **(USE CAUTION)**.

***

### DATAMINING
Basically, use **[Jedipedia.net](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)**'s tools and check our **[Discord](https://discord.gg/XfHFjSN)**. We'll see about adding new material, but this is very involved stuff.


***

### SWTOR TECHNICAL INFORMATION:
* File Formats:  
  (**32-bit. Needs updating to 64-bit**):
  * [Overview.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/File-Formats)
  * [gr2 Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/GR2-File-Structure)
  * [jba Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JBA-File-Structure)
  * [clo Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/CLO-File-Structure)
* [A look at SWTOR's Materials and Texture Files.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-materials-and-texture-files)

***

### OTHER RESOURCES:
* [Articles, lectures and talks about SWTOR's development.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Articles,-lectures-and-talks)
* [**Playing SWTOR on old Macs (x86) and Linux.**](https://github.com/SWTOR-Slicers/WikiPedia/wiki/playing-swtor-on-other-operating-systems)