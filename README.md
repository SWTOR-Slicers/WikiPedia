* ### We are now compatible with Blender 4.3 and higher.
* ### We have a workable solution to using SWTOR Game Update 7.6' new modernized skin materials. Please update both the .gr2 Importer and the ZG SWTOR Tools Add-ons.
* ### TORCommunity.com's Character Designer doesn't support selecting the new skin colors available with Game Update 7.7 or higher. That said, the colors can be recreated with our materials' Hue-Saturation-Brightness-Contrast controls, after the character has been assembled.

# Welcome to the SWTOR Slicers wiki!

We are a group of swtor fans who enjoy messing with the game and pulling out models, textures, etc. This GitHub repository contains tools and guides to help you do so yourself, as well as some other things.

In this Wiki we pool all the knowledge we are gathering on SWTOR's data and how to use it, be it to discover what Broadsword is cooking (datamining), to enhance our SWTOR experience by changing the game's looks (modding, sadly on hiatus at the moment as the tools need upgrading), or to make art out of the game's assets and immortalize our player characters through other 3D apps or even 3D-printing (extracting). Bear with us: it's far easier than it looks 🙂.

We encourage you to join our [**SWTOR Slicers Discord Server**](https://discord.gg/XfHFjSN), where you will be able to interact with fellow hobbyists in a direct manner, find help if you get stuck, and even contribute if you feel like it.

(You can find a few of us in the popular **SWTOR Artists Discord Server**'s 3d art channels, too)

***
(We do not condone the usage of our tools for malicious intent, including: **exploits**, **harassment of others**, or anything else that may violate EA/Bioware's [EULA](https://www.swtor.com/legalnotices/euala), [TOS](http://www.swtor.com/legalnotices/termsofservice), [DSA](https://www.swtor.com/legalnotices/digitalservicesagreement), [Privacy Policy](https://www.swtor.com/legalnotices/privacypolicy) Copyrights, Trademarks, or anything else illegal. We will not be held accountable for your actions, and will act against you if it becomes necessary)

***
* [Home.](https://github.com/SWTOR-Slicers/WikiPedia/wiki)
* **[State of Play May 2025](https://github.com/SWTOR-Slicers/WikiPedia/wiki/state-of-play)**
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
  **[Download](https://github.com/UltimaKaosXIII/extracTOR/releases/latest)** - **[User Guide](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ExtracTOR)**.
  
* **Blender (Windows/macOS/Linux app)**: popular free, open source 3D app.  
  **[Download](https://www.blender.org/download/lts/)** - **[User Guide](https://www.blender.org/support/)** - **[Short videoguides](https://www.youtube.com/playlist?list=PLa1F2ddGya_-UvuAqHAksYnB0qL9yWDO6)**


* **.gr2 Import/Export Add-on for Blender**: imports 3D models in SWTOR's .gr2 format.  
  **[Download](https://github.com/SWTOR-Slicers/Granny2-Plug-In-Blender-2.8x/releases/latest)** - **[User Guide](https://github.com/SWTOR-Slicers/Granny2-Plug-In-Blender-2.8x#swtor-granny2-gr2-importexport-add-on-for-blender-28-to-42)**.

* **ZG SWTOR Tools Add-on for Blender**: includes Character and Area Assemblers.  
  **[Download (incl. .gr2 Add-on)](https://github.com/SWTOR-Slicers/ZG-SWTOR-Tools/releases/latest)** - **[User Guide](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ZG-SWTOR-Tools-Add-on)**.

* **SWTOR Terrain Extractor (Windows command line executable)**: makes SWTOR terrain patches usable by our tools.  
  **[Download](https://github.com/UltimaKaosXIII/STE2/releases/latest)** - **[User Guide](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-Terrain-Extractor)**.

(Older tools like Slicers GUI, Noesis, or EasyMYP, are no longer needed, supported, or compatible at all)




### ONLINE TOOLS:

  * **[TORCommunity.com](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)**:  
  (warning: it runs VERY slowly)
    * [SWTOR Database](https://torcommunity.com/database/search/all) (with NPC Exporters).
    * [Character Designer](https://torcommunity.com/tools/character-designer).

  * **[Jedipedia.net](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)**:
    * [SWTOR Database](https://swtor.jedipedia.net/en).
    * [File Reader](https://swtor.jedipedia.net/reader).
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
    * [Locating weapons' assets manually.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
    * [Attaching weapons and other objects to a character **with a SWTOR rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character)
    * [Attaching weapons and other objects to a character **with a custom rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character-with-custom-rigs)
  
### Baking the models' textures and exporting to other apps:
  * Baking:
    * [Baking Legacy SWTOR materials and modern ones.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-models-to-export-them-to-other-apps)
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

* [Locating Player Characters' head assets through their Appearance Designer sliders data.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Understanding-In-Game-Head-Slider-Values)
* [Locating armor parts' assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-Armor-Parts-Assets)
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
**We have resumed modding tool development. Stay tuned for tools and tutorials.**
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