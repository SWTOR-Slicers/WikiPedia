### • Game Update 7.6 breaks our Character Assembler.
 It's meant to use the old skin textures, and the update only preserves a few of them. **DON'T OVERWRITE OR DELETE YOUR OLDER ASSETS EXTRACTION** (if you want to extract the update's new assets, do it to a separate folder). We are looking for a solution that allows to use both sets.

### • Blender 4.3 breaks our SWTOR materials-processing tools! Stay on 4.2 or older.
That said, **you can open 4.2 projects in 4.3** and the existing SWTOR materials will work (you can install as many versions of Blender you want at once and have them coexist without tripping each other).

### • New tool: [ExtracTOR](https://github.com/UltimaKaosXIII/extracTOR).
 **Meant to replace Slicers GUI**, it's a pure game assets extractor app by fellow slicer **[UltimaKaosXIII](https://github.com/UltimaKaosXIII)** that spares us the complications of the former tool. **You can take advantage of it already while we update these guides**.

*** 
# Welcome to the SWTOR Slicers wiki!

We are a group of swtor fans who enjoy messing with the game and pulling out models, textures, etc. This GitHub repository contains tools and guides to help you do so yourself, as well as some other things.

In this Wiki we pool all the knowledge we are gathering on SWTOR's data and how to use it, be it to discover what Broadsword is cooking (datamining), to enhance our SWTOR experience by changing the game's looks (modding, sadly on hiatus at the moment as the tools need upgrading), or to make art out of the game's assets and immortalize our player characters through other 3D apps or even 3D-printing (extracting). Bear with us: it's far easier than it looks 🙂.

We encourage you to join our [**SWTOR Slicers Discord Server**](https://discord.gg/XfHFjSN), where you will be able to interact with fellow hobbyists in a direct manner, find help if you get stuck, and even contribute if you feel like it.

(You can find a few of us in the popular **SWTOR Artists Discord Server**'s 3d art channels, too)

***
(We do not condone the usage of our tools for malicious intent, including: **exploits**, **harassment of others**, or anything else that may violate EA/Bioware's [EULA](https://www.swtor.com/legalnotices/euala), [TOS](http://www.swtor.com/legalnotices/termsofservice), [DSA](https://www.swtor.com/legalnotices/digitalservicesagreement), [Privacy Policy](https://www.swtor.com/legalnotices/privacypolicy) Copyrights, Trademarks, or anything else illegal. We will not be held accountable for your actions, and will act against you if it becomes necessary)

***
# Table of Contents
* [Home.](https://github.com/SWTOR-Slicers/WikiPedia/wiki)
* **[State of Play December 2024](https://github.com/SWTOR-Slicers/WikiPedia/wiki/state-of-play)**
* Getting Help:
  * [Link to the SWTOR Slicers Discord Server.](https://discord.gg/XfHFjSN)
  * [TORCommunity and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)
  * [Jedipedia and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)

***

### INTRODUCTION

 [**IMPORTING SWTOR MODELS INTO BLENDER: A BRIEF OVERVIEW**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-SWTOR-models-into-Blender-An-overview)  
  **Check this intro first. Afterwards, you can jump directly to the guides on extracting PCs, NPCs and others**. 

***

### TOOLS
**No need to read this section right now: each extracting/assembling guide explains its required tools anyway.**

#### Applications and Blender Add-on tools:
  * [Slicers GUI](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Installing-Slicers-GUI-and-extracting-SWTOR-game-assets) (Windows app).
  * [Blender 3D](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Blender) (multiplatform app):  
    **Which version. How to learn. Installing our Add-ons.**
  * [SWTOR .gr2 Objects Importer Add-on](https://github.com/SWTOR-Slicers/WikiPedia/wiki/gr2-Importer-Add‐on).  
  **Required by all the other add-ons**.
  * [SWTOR Character Assembler Add-on.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Character-Assembler-Add-on)  
  **(In maintenance. Use the ZG SWTOR Tools' version for now**)

  * [SWTOR Area Assembler Add-on](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assembling-SWTOR-Game-Areas-via-the-SWTOR-Area-Assembler-Addon-for-Blender).  
  (**In maintenance. Use the ZG SWTOR Tools' version for now**)
    * [SWTOR Terrain Extractor Command Line Tool](SWTOR-Terrain-Extractor).
  * [ZeroGravitas' ZG SWTOR Tools Add-on](https://github.com/SWTOR-Slicers/WikiPedia/wiki/ZG-SWTOR-Tools-Add-on).  
    **Includes the Character and Area Assemblers plus other diverse tools**.
    * [Installation and Status Panel](ZG-SWTOR-Tools-Installation-and-Status-Panel)
    *  [Area Assembler Tools](ZG-SWTOR-Area-Tools)
    *  [Character Assembler Tools](ZG-SWTOR-Character-Tools)
    *  [Materials Tools](ZG-SWTOR-Materials-Tools)
    *  [Objects Tools](ZG-SWTOR-Objects-Tools)
    *  [Pose And Sculpt Tools](ZG-SWTOR-Pose-and-Sculpt-Tools)
    *  [Baking Tools](ZG-SWTOR-Baking-Tools)

#### Online Tools:
  * [Jedipedia.net](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia):
    * SWTOR Database.
    * File Reader.
    * World Viewer.
  * [TORCommunity.com](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity):
    * SWTOR Database.
    * Character Designer.
    * NPC viewer's Exporter.
  
#### Deprecated Tools:
  * [EasyMYP](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-SWTOR-assets-with-EasyMYP) (Windows app).
  * Noesis (Windows app).

***

### THE COMPLETE GUIDE TO AUTO-EXTRACTING AND ASSEMBLING PLAYER CHARACTERS AND NPCs:

**[READ THE BROAD STROKES FIRST: YOU'LL SEE IT'S EASIER THAN YOU THINK!](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically)**
  * The steps:
    * [Installing Slicers GUI and extracting SWTOR's game assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Installing-Slicers-GUI-and-extracting-SWTOR-game-assets)
    * [Using TORCommunity's Character Designer to export Player Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-Character-Designer)
      * **IF ARMOR SELECTION SEARCH IS DOWN:** [workaround to manually specify Armor Sets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORC-Character-Designer-and-Manually-Creating-Armor-Sets)
    * [Using TORCommunity's NPCs Database to export Non Playable Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-NPCs-Database)
    * [Using our Blender add-ons to auto-assemble the model.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-the-character-with-the-Character-Assembler-Add-on)
    * [Rigging the character for posing and animation](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Binding-a-character-to-a-posing-skeleton)
    * [Applying SWTOR animations to the character.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Applying-SWTOR-animations-to-a-skeleton)  

* Extra steps that require manual work and some knowledge of SWTOR's assets:
    * [Making capes and hair work, manually and through Cloth Simulation.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Making-capes-and-hair-work,-manually-and-through-Cloth-Simulation)
    * [Locating weapons' assets manually.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
    * [Attaching weapons and other objects to a character **with a SWTOR rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character)
    * [Attaching weapons and other objects to a character **with a custom rig**.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character-with-custom-rigs)
  
  * Baking the models' textures and exporting to other apps:
    * [Baking with Legacy SWTOR materials and modern ones.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-models-to-export-them-to-other-apps)
    * [Baking the multiple materials of an object into a single one.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-multiple-materials-of-an-object-into-a-single-one)
    * [Exporting to VRChat.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-SWTOR-models-to-VRChat)
    * [Exporting to Star Wars Battlefront II.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-SWTOR-models-to-Battlefront-II)
    * Exporting to Unreal Engine.
    * [Exporting to Garry's Mod](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-to-Garrys-Mod-(GMod)).
    * Exporting to Tabletop Simulator.
  * 3D Printing:
    * [Baking Normals into real 3D detailing](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-Normals)

***

### ASSEMBLING GAME LOCATIONS AUTOMATICALLY:

* [Assembling SWTOR Game Areas with Jedipedia.net data and the SWTOR Area Assembler Addon](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assembling-SWTOR-Game-Areas-via-the-SWTOR-Area-Assembler-Addon-for-Blender).

***

### LOCATING AND ASSEMBLING ASSETS MANUALLY:

* [Locating armor parts' assets](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-Armor-Parts-Assets)
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

### MODDING (to do)
**Modding isn't working at the moment due to SWTOR's change to a 64bit codebase. It's going to take a while 🙁.**
* Overview.
* Tools.
* Other techniques:
  * [Modding SWTOR textures with Special K](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Modding-SWTOR-textures-with-Special-K) **(CAUTION)**.

***

### DATAMINING (to do)
* Overview.
* Tools.

***

### SWTOR TECHNICAL INFORMATION:
* File Formats (**32-bit. Needs updating to 64-bit**):
  * [Overview.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/File-Formats)
  * [gr2 Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/GR2-File-Structure)
  * [jba Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JBA-File-Structure)
  * [clo Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/CLO-File-Structure)
* [A look at SWTOR's Materials and Texture Files.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-materials-and-texture-files)

***

### OTHER RESOURCES:
* [Articles, lectures and talks about SWTOR's development.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Articles,-lectures-and-talks)
* [**Playing SWTOR on macOS and Linux.**](https://github.com/SWTOR-Slicers/WikiPedia/wiki/playing-swtor-on-other-operating-systems)
