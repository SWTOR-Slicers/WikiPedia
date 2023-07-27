## STATE OF PLAY JULY 2023:

### • Our two most basic tools (many of the rest depend on them) are almost but not yet fully compatible with files extracted from the recent SWTOR Game Update 7.2.1 onwards (SWTOR 64 bits):
* **Slicers GUI is usable: it both extracts and locates game assets in any version of SWTOR. As locating character assets is this bit buggy at the moment, we recommend using the [SWTOR Character Assembler Addon](https://github.com/SWTOR-Slicers/SWTOR-Character-Assembler) for this process, instead.**
* **The .gr2 Importer Addon is half-way there: it imports objects and applies materials correctly, but the handling of skeletons and animations from SWTOR 64 bits is yet to be solved.**

  **It can import older SWTOR 32 bits versions of those, though. If you need these last specific features, you could replace the related assets with the ones extracted from a SWTOR previous to the Game Update (whose files you can download from [here](https://drive.google.com/drive/folders/1ZkBNz1cK_IXBxBd4OIYL1jRImnnfHXKW?usp=sharing)).**

### • Modding tools don't work yet with SWTOR 64 bits.

### • New Tool: the [SWTOR Character Assembler Blender Addon](https://github.com/SWTOR-Slicers/SWTOR-Character-Assembler):  
It combines in a single button operation the character asset-locating function of Slicers GUI and the actual importing into Blender described in the **[Guide to Auto-Extracting and Assembling Player Characters](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically)**, adding a few options of its own. More information and link in that guide.

### • TORCommunity.com's Character Designer's armor search works again!

### • TORCommunity.com's NPC Database's 3D viewer and exporter is down:
We have a temporary stash of old exported NPC definition files in the Discord Server which might contain the NPC that you are interested in.

___


# Welcome to the SWTOR Slicers wiki!

We are a group of swtor fans who enjoy messing with the game, and pulling out models, textures, etc. This GitHub repository contains tools and guides to help you do so yourself, as well as some other things.

In this Wiki we pool all the knowledge we are gathering on SWTOR's data and how to use it, be it to discover what the game developers are cooking (**datamining**), to enhance our SWTOR experience by changing the game's looks (**modding**), or to make art out of the game's assets and immortalize our player characters through other 3D apps or even 3D-printing (**extracting**)!

We realize the information and guides we present here might be a little overwhelming. It's getting far, _far_ better: the Slicers gang is building simpler, easier tools that keep all the drudgery down to a minimum. Still, it's good to know what's what and where it is, because it allows for interesting experimentation.

There's much to add to this guide yet. We'll be filling the holes and updating its content as new tools and methods arise, so, keep an eye on it. Also, we encourage you to join our [**Discord Server**](https://discord.gg/XfHFjSN), where you will be able to interact with fellow hobbyists in a direct manner, find help if you get stuck, and even contribute if you feel like it.

### If your main interest is recreating your Player Characters or your favorite NPCs in [Blender](https://blender.org/), the popular, free 3D app, or use it as an intermediate step to bring them to other apps, we can direct you straight to [this guide on how to do it in the most automated, hassle free way so far](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically).

---
(We do not condone the usage of our tools for malicious intent, including: **exploits**, **harassment of others**, or anything else that may violate EA/Bioware's [EULA](https://www.swtor.com/legalnotices/euala), [TOS](http://www.swtor.com/legalnotices/termsofservice), [DSA](https://www.swtor.com/legalnotices/digitalservicesagreement), [Privacy Policy](https://www.swtor.com/legalnotices/privacypolicy) Copyrights, Trademarks, or anything else illegal. We will not be held accountable for your actions, and will act against you if it becomes necessary)


***

Last update: 27 Jul, 2023
*  **Revised Player Character/NPC Importing guide based on new tools**

***
# Table of Contents
* [Home.](https://github.com/SWTOR-Slicers/WikiPedia/wiki)
* Getting Help:
  * [Link to the SWTOR Slicers Discord Server.](https://discord.gg/XfHFjSN)
  * [TORCommunity and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)
  * [Jedipedia and its online tools.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)

***

### THE COMPLETE GUIDE TO AUTO-EXTRACTING AND ASSEMBLING PLAYER CHARACTERS AND NPCs:
  * [Read the broad strokes first: you'll see it's easier than you think!](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically)
  * The steps:
    * [Installing Slicers GUI and extracting SWTOR's game assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Installing-Slicers-GUI-and-extracting-SWTOR-game-assets)
    * [Using TORCommunity's Character Designer to export Player Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-Character-Designer)
      * **NO LONGER NEEDED!** [TORC Character Designer armor selection workaround: Manually Creating Armor Sets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORC-Character-Designer-and-Manually-Creating-Armor-Sets)
    * [Using TORCommunity's NPCs Database to export Non Playable Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-NPCs-Database)
    * [Using our Blender add-ons to auto-assemble the model.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-the-character-with-the-Character-Assembler-Add-on)
    * [Rigging the character for posing and animation](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Binding-a-character-to-a-posing-skeleton)
    * [Applying SWTOR animations to the character.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Applying-SWTOR-animations-to-a-skeleton)  

* Extra steps that require manual work and some knowledge of SWTOR's assets:
    * [Making capes and hair work, manually and through Cloth Simulation.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Making-capes-and-hair-work,-manually-and-through-Cloth-Simulation)
    * [Locating weapons' assets manually.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
    * [Attaching weapons and other objects to a character.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Attaching-weapons-and-other-objects-to-a-character)

  * Baking the models' textures and exporting to other apps:
    * ["Baking" with Legacy SWTOR materials and modern ones.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-the-models-to-export-them-to-other-apps)
    * [Exporting to VRChat.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-SWTOR-models-to-VRChat)
    * Exporting to Unreal Engine.
    * [Exporting to Garry's Mod](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Exporting-to-Garry-Mod-(GMod)).
    * Exporting to Tabletop Simulator.
  * 3D Printing:
    * [Baking Normals into real 3D detailing](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Baking-Normals)

***
### ASSEMBLING GAME LOCATIONS AUTOMATICALLY:

* [Assembling SWTOR Game Areas with Jedipedia.net data and the SWTOR Area Assembler Addon](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assembling-SWTOR-Game-Areas-via-the-SWTOR-Area-Assembler-Addon-for-Blender).

### LOCATING AND ASSEMBLING ASSETS MANUALLY:

* [Locating armor parts' assets](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-Armor-Parts-Assets)
* [Locating weapons' assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Locating-weapons-assets)
* [Assigning materials and textures to environmental and architectural elements, furniture, props, ships, vehicles and weapons.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assigning-materials-and-textures-to-environmental-and-architectural-elements,-furniture,-props,-ships,-vehicles-and-weapons)
* [Assembling multi-part assets (Decorations, Rooms, etc).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Assembling-Multi-Part-Assets-(Decorations,-Rooms,-etc))
* [Generic guide to importing objects and assigning materials (**Legacy Add-on-based**. Needs updating).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Importing-Objects-and-Assigning-Materials-in-Blender)

***

### OTHER GUIDES:

  * [Snippets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Snippets)
  * Improving and customizing our SWTOR models and materials.
    * [List of tips and tricks to cover in the future.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Blender-and-SWTOR-Tips-and-Tricks)
    * [Replacing body parts with gear vs. putting gear on top of body parts](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Replacing-body-parts-with-gear-vs.-putting-gear-on-top-of-body-parts)
    * [Merge by Distance before applying Modifiers.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Merge-by-Distance-before-applying-Modifiers)
    * [Enhancing SWTOR texture maps with Cupscale.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Enhancing-SWTOR-texture-maps-with-Cupscale)
  * [Other Extracting Strategies (needs updating).](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-strategies)
  * SWTOR Materials recipes:
    * [SWTOR’s holosigns: how to make them work in Blender.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-holographic-signs:-how-to-make-them-work)
***

### MODDING (to do)
* Overview.
* Tools.

***

### DATAMINING (to do)
* Overview.
* Tools.

***

### AVAILABLE TOOLS (needs updating)

* [Tools overview.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Tools-overview)
* Slicers GUI: unified tool for viewing, extracting, converting and modding SWTOR assets and data:
  * [Slicers GUI overview.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Slicers-GUI-overview)
  * [Installation.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Slicers-GUI-Installation)
  * [Extracting SWTOR's assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-SWTOR-assets-with-the-Slicers-GUI)
  * Viewing and converting extracted assets.
* EasyMYP: tool for extracting SWTOR assets (OBSOLETE if still useful. We recommend using Slicers GUI instead):
  * [Extracting SWTOR's assets with EasyMYP.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-SWTOR-assets-with-EasyMYP)
* Noesis: assets viewer and converter (OBSOLETE FOR MODEL CONVERSIONS. We recommend using Blender and our .gr2 importer add-on instead):
  * Noesis overview.
  * Viewing assets with their textures (at times) with Noesis.
  * Converting SWTOR models (badly) and "unpacking" their textures.
  * Batch-converting SWTOR models (painfully).
  * Batch-converting SWTOR textures. 

***

### SWTOR TECHNICAL INFORMATION:
* File Formats
  * [Overview.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/File-Formats)
  * [gr2 Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/GR2-File-Structure)
  * [jba Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JBA-File-Structure)
  * [clo Structure.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/CLO-File-Structure)
* [A look at SWTOR's Materials and Texture Files.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/SWTOR-materials-and-texture-files)

***

### OTHER RESOURCES:
* [Articles, lectures and talks about SWTOR's development.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Articles,-lectures-and-talks)
* [**Playing SWTOR on MacOS and Linux.**](https://github.com/SWTOR-Slicers/WikiPedia/wiki/playing-swtor-on-other-operating-systems)
