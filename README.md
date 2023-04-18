## WARNING: our tools aren't yet fully compatible with files extracted from the recent SWTOR Game Update 7.2.1:
* **Slicers GUI is usable: version 1.12.0 both extracts and locates game assets.**
* **The .gr2 Importer Addon is half-way there: it imports objects and applies materials correctly, but the handling of skeletons and animations is yet to be solved.**

**If you need these last specific features, you could keep on using the older versions of the tools on assets from a SWTOR previous to the Game Update, which you can download from [here](https://drive.google.com/drive/folders/1ZkBNz1cK_IXBxBd4OIYL1jRImnnfHXKW?usp=sharing)).**
___


### If your main interest is recreating your Player Characters or your favorite NPCs in [Blender](https://blender.org/), the popular, free 3D app, or use it as an intermediate step to bring them to other apps, we can direct you straight to [this guide on how to do it in the most automated, hassle free way so far](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically).

## Welcome to the SWTOR Slicers wiki!

We are a group of swtor fans who enjoy messing with the game, and pulling out models, textures, etc. This GitHub repository contains tools and guides to help you do so yourself, as well as some other things.

This Wiki is where we pool all the knowledge we are gathering on SWTOR's data and how to use it, be it to discover what BioWare is cooking (datamining), to enhance our SWTOR experience by changing the game's looks (modding), or to make art out of the game's assets and immortalize our player characters through other 3D apps or even 3D-printing (extracting)!

We realize the information and guides we present here might be a little overwhelming. It's getting far, _far_ better: the Slicers gang is building simpler, easier tools that keep all the drudgery down to a minimum. Still, it's good to know what's what and where it is, because it allows for interesting experimentation.

There's much to add to this guide yet. We'll be filling the holes and updating its content as new tools and methods arise, so, keep an eye on it. Also, we encourage you to join our [**Discord Server**](https://discord.gg/XfHFjSN), where you will be able to interact with fellow hobbyists in a direct manner, find help if you get stuck, and even contribute if you feel like it.

(We do not condone the usage of our tools for malicious intent, including: **exploits**, **harassment of others**, or anything else that may violate EA/Bioware's [EULA](https://www.swtor.com/legalnotices/euala), [TOS](http://www.swtor.com/legalnotices/termsofservice), [DSA](https://www.swtor.com/legalnotices/digitalservicesagreement), [Privacy Policy](https://www.swtor.com/legalnotices/privacypolicy) Copyrights, Trademarks, or anything else illegal. We will not be held accountable for your actions, and will act against you if it becomes necessary)


***

Last update: 13 Oct, 2022
*  **New guide by RandomUser: how to make SWTOR's street holosigns textures work in Blender.**

***

# Table of Contents
* [Home.](https://github.com/SWTOR-Slicers/WikiPedia/wiki)
* Getting Help:
  * [The SWTOR Slicers Discord Server.](https://discord.gg/XfHFjSN)
  * [TORCommunity.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORCommunity)
  * [Jedipedia.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/JediPedia)

***

### THE COMPLETE GUIDE TO AUTO-EXTRACTING AND ASSEMBLING PLAYER CHARACTERS AND NPCs:
  * [Read the broad strokes first: you'll see it's easier than you think!](https://github.com/SWTOR-Slicers/WikiPedia/wiki/locating-swtor-characters-assets-automatically)
  * The steps:
    * [Installing Slicers GUI and extracting SWTOR's game assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Installing-Slicers-GUI-and-extracting-SWTOR-game-assets)
    * [Using TORCommunity's Character Designer to export Player Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-Character-Designer)
      * **NO LONGER NEEDED!** [TORC Character Designer armor selection workaround: Manually Creating Armor Sets.]([https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORC-Character-Designer:-Manually-Creating-Armor-Sets](https://github.com/SWTOR-Slicers/WikiPedia/wiki/TORC-Character-Designer-and-Manually-Creating-Armor-Sets))
    * [Using TORCommunity's NPCs Database to export Non Playable Characters.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-TORCommunity-NPCs-Database)
    * [Gathering the character's assets with the Slicer GUI tool.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Gathering-the-character-assets-with-the-Slicer-GUI-tool)
    * [Using Blender and the SWTOR importer add-on to auto-assemble the model.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Using-Blender-and-the-SWTOR-importer-add-on-to-auto-assemble-the-model)
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
  * [Extracting SWTOR's assets.](https://github.com/SWTOR-Slicers/WikiPedia/wiki/Extracting-SWTOR's-assets-with-the-Slicers-GUI)
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
