# SWTOR Extractors, Modders, and Dataminers WikiPedia

introduction...


## Table of Contents

| Sections  | Sections |
| :---: | :---: |
| [Overview](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#overview)  | [Datamining](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#datamining)  |
| [Extracting](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#extracting)  | [Resources](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#resources)  |
| [Modding](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#modding)  | [Getting Help](https://github.com/SWTOR-Extractors-Modders-Dataminers/WikiPedia#getting-help)  |


## Overview

## Extracting

### Section Contents

| Topics | Topics |
| :---: | :---: |
| EasyMYP | Locating files |

### Extracting SWTOR's Resources With EasyMYP

EasyMYP is a game assets extracting tool. There is an specific SWTOR-compatible version, sometimes alluded to as "TorMYP", which allows us to inspect SWTOR's .tor asset files, extract specific items or groups of items from them, and even extract the assets of a whole folder of .tor files in one go.

EasyMYP can be downloaded from [this repository](https://github.com/SWTOR-Extractors-Modders-Dataminers/EasyMYP).

To be of use, we'll need to download the most current hashes file (a file holding the list of currently identified game objects and their IDs) from [here](https://drive.google.com/drive/folders/1VmoAOY9EM12BV5qeWkiAHaef6nDR0XBT). *hashes\_filename.zip* is the one meant for EasyMYP. Decompress the .zip file to get the *hashes\_filename.txt* file.

(it might be convenient to download *hashes\_filename.bin.gz*, too, as it is used in other tools we'll see about later on when assembling the assets in 3D apps).


#### The EasyMYP tool

EasyMYP, once unzipped, appears as a single folder that can be placed anywhere in our computers (such as, for example, the desktop folder), no installation process needed. Its interesting bits are:

<img align="left" src="images/extracting/easymyp/easymyp_guide_010.png">

- **EasyMYP.exe**: that's the app as such.

- **Hash**: this folder is were we place the hashes\_filename.txt file, which contains a list of all the game assets that have been identified to date. This file is usually posted by fellow dataminers every time there is a new game update (not just the major ones but minor ones that introduce new Cartel Market armor gear and the like, too). There are hash file releases for the Public Test Server, too.
We can simply drop the file inside the folder and overwrite any older hash file without care.

- **EasyMYP.config**: a human-readable XML file where the app stores its preferences settings. It can be useful to read at times, because it stores the destination folder where the extracted files will be placed, and the app is this bit inconsistent in setting that (there's two ways of doing it, and sometimes I have seen TorMYP show different information for each).

- **README.txt**: the app's instructions. They show up inside the app through the help menu, too.

Every time we launch EasyMYP.exe, we'll see first a brief progress bar showing that it is reading the contents of the hash file. Once done, it'll show its simple interface. Of the many options the app has, we'll use just a few ones, mainly in Archive and Files.

<br/><br/><br/>
![](images/extracting/easymyp/easymyp_guide_020.png)

#### Extracted items' destination

An important decision to take is where to store the results of its usage, for the following reason: when exporting assets, EasyMYP won't simply ask us where to save them and then leave the files there. What it'll do is recreate the game's internal assets organization inside the folder we choose, which can easily become six or more sublevels deep. For example, the player characters' eye textures will end up located at: *your chosen folder > resources > art > dynamic > player\_character > face\_customization > eye*.

(Don't let that scare us into thinking that finding the extracted material inside that mess will be difficult. On the contrary: Windows and macOS' instant desktop search is our most excellent friend, and most of times we won't have to care for the directory path at all)

So, we start by telling EasyMYP where we want to store all the extracted stuff through File > Select Extraction Folder. If we would happen to forget to do it, the app will ask us the first time we do an extraction, anyway. It can be set through the Options menu, too. Ultimately, it can even be set by opening the EasyMYP.config file in Notepad and typing the folder's directory path.

![](images/extracting/easymyp/easymyp_guide_030.png)

#### Opening and exploring the game's asset files

In Windows 10 those are typically stored at C:\Program Files (x86)\Electronic Arts\BioWare\Star Wars - The Old Republic\Assets (now that SWTOR is being published through Steam, too, they could be stored somewhere else depending on our Steam preferences).

There, we'll find a lot of files with the .tor extension and fairly informative names.

![](images/extracting/easymyp/easymyp_guide_040.png)

The most interesting files are the ones containing an "art" in their names:

- Filenames starting with “swtor\_main\_art\_dynamic\_”: those contain body parts and armor parts the game builds our characters and companions out of. These are the ones we will be most interested in if we want to do character-related stuff.

- Filenames containing the "\_creature\_" word: those refer to beasts, characters and others that are built as full body single meshes: say, an early Darth Malgus, an Akk dog.
 
- Filenames starting with “swtor\_main\_area\_” and “swtor\_main\_art\_area\_”: they contain terrain and buildings’ parts: whole mountains, bridges, buildings and empty rooms; or “construction sets” involving walls, furniture, road parts, etc. It holds spaceship interiors and exteriors, too. Don't confuse them with the ones starting with "swtor\_en-us\_area\_" without the "\_art\_", as those don't contain any such asset.

- Other filenames containing the "\_art\_" word: we can find in them weapons, ships, vehicles, "farming" items (crystals, crates, etc.).

The rest of the stuff relates to game audio and conversations ("\_bnk\_"), animation and FX scripts ("\_anim\_"), user interface art ("\_gfx\_") such as all the Galactic Trade Network and Cartel Market images, abilities icons, etc., maps, etc. They are quite interesting, actually, but we can omit them and save a lot of hard disk space.

Let's see how the app works with these files. Let’s say we open "swtor\_main\_art\_creature\_b\_1.tor", which ought to contain a few animals from the game. Get to Archive > Open Archive, navigate to SWTOR’s Assets folder and open that file.

![](images/extracting/easymyp/easymyp_guide_060.png)

After a few seconds of processing (no progress bars 😕 ), it’ll show up in the left side pane:

![](images/extracting/easymyp/easymyp_guide_070.png)

We can see the contents of the file by clicking on the Archive File List tab, but it’s more interesting to see them by twirling the little + widget at its left, because it’ll show them in their hierarchical organization structure, which will reflect how they will be saved in the extraction folder that we chose (or will choose the first time we do an export).

![](images/extracting/easymyp/easymyp_guide_080.png)

Out of that first twirl, we’ll see that there’s a lot of files with unintelligible names, and a folder. The former are assets in that .tor file that we still don’t know what they are (they are not in the hash file yet). Those can be saved and examined: EasyMYP will put them in a subfolder with the same name as the .tor file so that things aren’t too messy.

It’s that lone folder where the really interesting stuff starts:

![](images/extracting/easymyp/easymyp_guide_090.png)

What we see here are folders where models (.gr2 archives) and textures (.dds archives) are stored. We can begin to get a feel of how things are organized: the “dynamic” folder contains all elements that are animated in the game. The “materials” one contains text files describing what textures correspond to which models, etc.

![](images/extracting/easymyp/easymyp_guide_100.png)

We should warn you that Bioware isn’t the tidiest developer ever: sometimes things are a bit disorderly, surely out of adding things to the game in ways they hadn’t anticipated before launch.

(By the way, we can open several .tor files during the same session and explore them all this way)

![](images/extracting/easymyp/easymyp_guide_140.png)

### Exporting specific assets and groups of assets

So, we might want to export a single item:

![](images/extracting/easymyp/easymyp_guide_110.png)

Or a bunch of items: a whole folder, for example, which is better because sometimes the meshes and textures are in the same folder although grouped into subfolders.

![](images/extracting/easymyp/easymyp_guide_120.png)

Or one could just extract all the contents of the .tor file and decide what to keep and what to delete afterwards.

![](images/extracting/easymyp/easymyp_guide_130.png)


### Exporting several whole .tor files' assets in one go

Sadly, all this isn’t the most efficient way to work if we look forward to building whole scenes with landscapes, rooms, props, pets, characters, etc., or even if we just want to recreate our player characters. At first, we used to suggest extracting the stuff from just a type of files (the character parts ones, or the architectural ones, etc.), but, frankly, everything is so spread around that one always ends up missing something and losing massive amounts of time trying to locate it.

Given that, it’s best to just batch-export all the .tor files having to do with 3d models (well, maybe we can leave the "\_area\_" ones out if we don't plan on using the game's buildings and exteriors). 

EasyMYP has an option to extract the stuff inside all the .tor files contained in a folder:

![](images/extracting/easymyp/easymyp_guide_150.png)

A batch extraction of all the 3D models and related files will fill some 40-50 GB. An extraction of just *everything*, including audio files, GTN items’ icons, maps, etc. will fill about 100 GB.

How do we separate the .tor files we want to process from the ones we don’t? By temporarily putting them inside a folder (inside Assets or somewhere else), processing them, and putting them back into Assets afterwards.<u><br></u>

![](images/extracting/easymyp/easymyp_guide_160.png)

So, we click on “Extract All from Folder”. TorMYP will ask we where that folder is, and we point it at it.

![](images/extracting/easymyp/easymyp_guide_170.png)

Then it asks us a curious question:

![](images/extracting/easymyp/easymyp_guide_180.png)

What does this mean? EasyMYP is offering us to extract everything (“No” option 🤨) or only the XML text files describing how the assets are organized (“Yes” option): those .xml files tell us, for example, which objects are used to build, say, a chest armor piece, and where they are and what material file is associated with them… which in turn will tell us which texture files it uses and where they are, and what color scheme file is applicable… which in turn will describe what colors the armor will use because oftentimes a same armor object shows up as different items just by changing some colors…

So, we choose "no".

(That said, maybe afterwards we might want to do a second, .xml files-only extraction, from all .tor files, saying “Yes”. These don’t ocuppy much space, help build the whole subfolder organization, and you get the certainty that you have all the .XML information about all the game assets at your fingertips just in case)

Before proceeding, EasyMYP will show a dialog window telling us what’s about to do, giving us a chance to backtrack. Then it’ll start going .tor file by .tor file. They’ll accumulate in the left side pane, which is a way to measure its progress.

![](images/extracting/easymyp/easymyp_guide_190.png)

A warning, though: sometimes EasyMYP crashes while processing the biggest of those files, so, it's good to keep an eye on its progress. If it happens to crash, we can move the files it already processed out of the temporary folder and back to the Assets one, then relaunch the operation. If we didn’t happen to see in which one the crash occurred, a trick to know it is to look at the contents of the folder storing the results: there ought to be subfolders with the same names as the .tor files it has processed. Just check which was the last one, and restart from there.

This might be a memory issue. We've seen it happen in PCs with 16 GB. of RAM, and the crash usually happens when extracting the first of the big files holding the game's audio ("swtor\_main\_bnk\_audio\_1.tor"), so, it might be prudent to move those to another temporary folder to process them as a second batch job or just dismiss them.

### The results of the extraction and saving some storage space

<img align="left" src="images/extracting/easymyp/easymyp_guide_200.png">

Once we are done, we can find ourselves with literally thousands of files inside a complex folder structure (a merge of all the subfolders contained in each .tor file) which can be a bit overwhelming. Actually, handling it will be far easier than it looks, because most of times we will be copypasting filenames and the like into Windows' instant search's field, and it will show us not just found filenames but, even more importantly, found .xml files mentioning those filenames without the need to dig deep inside the subfolders tree.

As we mentioned before, the really juicy stuff is in the *resources* folder. The others, named like the .tor files, contain assets whose IDs aren't known yet. They *can* be useful if there is something (an object, a texture file, etc.) that we *know it should be somewhere in there* but can't be found: we can try those folders with a model viewer such as [Noesis](https://github.com/SWTOR-Extractors-Modders-Dataminers/NOESIS) or a free .dds format image viewer such as [XnView](https://www.xnview.com/) or [Noesis]([Noesis](https://github.com/SWTOR-Extractors-Modders-Dataminers/NOESIS)) too. Then again, they could as well be deleted to free hard disk space.

Another measure to free storage space (and to ease browsing through the folders) is to delete the lower polygon count versions of the objects and their associate textures (they are used when they are far away from us in the game). These objects' filenames end in ".lod.gr2", and their textures end in ".tiny.dds". To select them through Windows' desktop search you can copypaste these queries in the search field and delete the results:

".lod.gr2" ext:gr2

".tiny.dds" ext:dds

The "ext:" bit makes sure that you are selecting the mesh and texture files and not any text file that could have been mentioning them. A warning: Windows can take its sweet time to select them all and to make a deletion: we are talking thousands of files. It's better to directly delete them instead of first moving them to the trashcan and then emptying it.

Now that we have the game assets extracted, it's time to learn how to find the ones we need to assemble characters, armor, weapons, vehicles, and environments.









### Importing the models into Blender with the .gr2 add-on

<<<<<<< HEAD
If you followed older guides based on the use of Noesis to convert SWTOR assets to usable formats (.obj 3D files and .png image ones, tipically), be aware that we no longer need such conversions thanks to LeeThorogood's .gr2 import/export add-on for Blender, the 3D app of choice out of both its ample capabilities and zero cost.
=======
If you followed older guides based on the use of Noesis to convert SWTOR assets to usable formats (.obj 3D files and .png image ones, tipically), be aware that we no longer need such conversions thanks to [LeeThorogood's .gr2 import/export add-on for Blender](https://github.com/SWTOR-Extractors-Modders-Dataminers/Granny2-Plug-In-Blender-2.8x), the 3D app of choice out of both its ample capabilities and zero cost.
>>>>>>> 37df7574dd3f34fa1e7f53f5b87c30dd90724227

Also, there is no need to modify the texture files in Photoshop or similar packages: Blender understands the .dds image format (it's pervasive in videogame production), and the preset materials provided by this same add-on do all the required texture manipulations.

So, Noesis is no longer necessary, although it still is useful as a model visor and, in certain cases, as a model and texture converter for less capable 3D apps.

#### Installation

This add-on's installation follows Blender's coventions for such a thing: download the add-on .ZIP file, DON'T decompress it, and install it via Edit menu > Preferences > Add-ons > Install. Activate it by clicking on its checkbox (no need to relaunch Blender) and it'll show up in the File menu >Import and Export submenus:

![](images/extracting/gr2-addon/gr2_addon_guide_010.png)

Its single importing option is the "Import Collision Mesh" checkbox, which normally will be left unchecked.





### Using the .gr2 add-on's SWTOR materials

Let's suppose we have imported the parts of a character. They'll appear correctly positioned already.

![](images/extracting/gr2-addon/gr2_addon_guide_030.png)

![](images/extracting/gr2-addon/gr2_addon_guide_020.png)

<img align="left" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_040.png">

If we happen to switch the Outliner to Blender File mode (no real need, but it is interesting), we'll notice that there are a series of new material "templates" added to the project: Creature, Eye, Garment, HairC, SkinB, and Uber (they are produced by the add-on the moment it imports a .gr2 file). Those names match the <derived> label that appears at the heading of the .mat material definition files, which tells us which one we'll use for each object.

We'll notice, too, that some of the materials have names that match the name of the .mat files, but some didn't manage that and defaulted to "default" and similar. That is a current limitation of the importer add-on. It's not really a problem because we are going to disregard those materials, replacing them with copies of the templates.

In the Outliner, twirling the objects' little left-side arrows, we can see their meshes and materials (and vertex groups, which aren't relevant for this tutorial).

<img align="right" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_050.png">

We see that sometimes there are two materials in an object instead of a single one. That usually happens in three cases:

<<<<<<< HEAD
* • A head that has a skin material and an eyes material.
* • A "hair piece" such as a Zabrak's horn plus hair object, which has materials for the hair and the horns.
* • A piece of armor that shows skin. As SWTOR replaces whole body parts with corresponding pieces of armor, those need to incorporate the skin of the body part they replace, which uses its own material.
=======
* A head that has a skin material and an eyes material.
* A "hair piece" such as a Zabrak's horn plus hair object, which has materials for the hair and the horns.
* A piece of armor that shows skin. As SWTOR replaces whole body parts with corresponding pieces of armor, those need to incorporate the skin of the body part they replace, which uses its own material.
>>>>>>> 37df7574dd3f34fa1e7f53f5b87c30dd90724227

In such cases, we would replace each of those materials with the relevant template ones. Say, the head body part would use the SkinB Shader for the first material and the Eye Shader for the second one. 

Let's go for the chest part as an example. In Blender's Shader Editor panel we see that the chest has been assigned a generic material based on the usual Principled BSDF shader (Blender goes to that one because it's kind of a Swiss Army knife shader)

![](images/extracting/gr2-addon/gr2_addon_guide_055.png)

We are NOT going to use that default material: what we are going to do is replace it with one of the template materials that the add-on created in the project at the moment of importing the model. As typical of any bare skin body part (or bit of skin showing in any piece of sexy armor), the .mat file tells us that we have to use a "SkinB" shader (that shows up as "<Derived>SkinB</Derived>" near the head of the file). We'll explain how to locate and interpret such files in another section of this Wiki.

![](images/extracting/gr2-addon/gr2_addon_guide_060.png)

So, with the object selected and the Shader Editor showing its material, we use the materials menu to select the SkinB Shader template. This will result in the replacement of the original material assignment with the SkinB Shader one.

![](images/extracting/gr2-addon/gr2_addon_guide_070.png)

BUT!!! We need to do something before continuing: yes, the materials are named "template" this and that, but Blender has no template library system as such (there is one doing trials in the latest betas), so we need to make a duplicate to preserve the original. If we don't, we risk finding ourselves rewriting and using the same material in different body parts without meaning to.

For that, we'll simply click on the New Material button next to the material name in the menu:

![](images/extracting/gr2-addon/gr2_addon_guide_080.png)

As the name field is so narrow, we probably won't see that clearly that the name was appended a ".001" or similar. We can check it by opening the wider selection menu, or by double-clicking the field (the cursor will move to the end of the name, so it will become visible).

![](images/extracting/gr2-addon/gr2_addon_guide_090.png)

Once having assigned this duplicate of the template to the object, it's best that we change that name to something more comprehensible. Say, "Chest".

![](images/extracting/gr2-addon/gr2_addon_guide_100.png)

#### Applying textures and values to the character's materials

Now, let's give the material a look. We can see that there is a big custom node (Node Group, in Blender's parlance) at the right side of the material's nodes network, and a lot of unassigned texture file nodes, named with the texture file suffixes that belong in each (ending in "_d", "_s", etc.) and the technical names BioWare gave them ("RotationMap" for normal maps, "PaletteMaskMap" for dye masks, etc).

![](images/extracting/gr2-addon/gr2_addon_guide_110.png)

Well: the idea is that you click on their "Open" buttons, browse to the correspondingly
suffixed files, and load them.

![](images/extracting/gr2-addon/gr2_addon_guide_120.png)

![](images/extracting/gr2-addon/gr2_addon_guide_130.png)

One thing we'll have to do to each of those, once assigned, is set their Color Space setting to "Raw" (Blender defaults them to sRGB, which isn't appropriate for the way these SWTOR materials work, especially in the case of non-image texture files such as the "_n" normal maps).

![](images/extracting/gr2-addon/gr2_addon_guide_140.png)

As the SkinB shader works for head body parts too, it includes nodes for Complexions and FacePaints (tattoos, fur patterns, etc.). The .mat file will tell you what to use in those nodes when dealing with non-head parts, using files such as "white", "default_facemap", etc.

(Currently, the SkinB Shader material doesn't support scar or wrinkles maps. We are looking into that)

#### The problem with character's color data

Now that we have all the texture files assigned, we can see about filling the big node group's fields with the data necessary to reproduce the colors and finish of the character. Most of it is in the .mat files, and its labelling matches the one in the node, but some of it isn't, most specifically the skin color (which happens to be the most important one, isn't it?). We'll see to it.

<img align="left" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_150.png">

The Palette1's X, Y, Z, and W fields are meant to work very much like Photoshop's (or any other painting app's) Hue-Saturation-Lightness adjustment tool. The fields are:

* Palette1.X = Hue adjustment.
* Palette1.Y = Saturation adjustment.
* Palette1.Z = Brightness adjustment.
* Palette1.W = Contrast adjustment.

The thing is: if we can't get the correct values (we can: it's just a bit involved), we can still eyeball them. We could start by raising Palette1.Z (brightness) to something like, say, 0.2, and Palette1.W (contrast) to 0.5, so that the object shows something other than black, and then we would play with all the Palette fields to try to approximate the skin color we want (shift-click'n'drag on those fields lets us change them in fine increments/decrements). Mind that Saturation (Palette1.X) is highest at 0 and lowest at 1, contrary to the usual.

<img align="right" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_160.jpg">

As for the Palette1 Specular and Metallic Specular, the corresponding data in the .mat files comes as value triplets, but we can see in the node that there are color wells instead of groups of fields. No trouble: we just open them and enter the values as R, G, B (and Alpha if there is a fourth value listed).

Let's see now about getting the actual, exact values for the Palette1 fields.

The problem we have is that, although most of the information about the objects' materials is present in the .xml and .mat files extracted with EasyMYP, there are bits that only exist in the game's nodes database, a non-human readable binary file, so we need NodeViewer to consult it (and maybe extract it to have it more at hand).

In NodeViewer, the skin, eye and hair's colors appear in the dynamic menu's related submenus: inside them, their nodes' names are the filenames that supposedly ought to exist in the EasyMYP extraction but, alas, don't.

![](images/extracting/gr2-addon/gr2_addon_guide_180.png)

For example, in the case of this Zabrak character, we can find the node and see there the Palette information we need. Note that the order of the fields in NodeViewer doesn't match the order in Blender's node, so remember what's what to place the values correctly:

* Palette1.X = appPaletteHue (hue adjustment).
* Palette1.Y = appPaletteSaturation (saturation adjustment).
* Palette1.Z = appPaletteBrightness (brightness adjustment).
* Palette1.W = appPaletteContrast (contrast adjustment).

(You can find there the Specular and MetallicSpecular values, too)

If a value appears with a minus sign and the results look weird, try omitting the sign (not yet fully sure about this but it seems to work).

![](images/extracting/gr2-addon/gr2_addon_guide_190.png)

For the material to handle transparency (typical of fine edge detail such as hair strands) while using the Eevee renderer, check that both the material's Blend Mode and Shadow Mode are set to "Alpha Clip". The latest version of the add-on ought to do that automatically.

![](images/extracting/gr2-addon/gr2_addon_guide_200.png)

And that's it, mostly.

#### Some issues regarding this add-on on different Blender versions

The current version of the .gr2 importer works in both Blender 2.8x and 2.9x, but the materials of a project started in 2.8x won't fully work in Blender 2.9x without some minor modifications: Blender introduced a new input socket in 2.9x' Principled Shader between the "Emission" and the "Alpha" ones, and that makes some of the materials' shader network "noodles" connect to the wrong inputs. It's easy to correct manually and we'll add a small guide to how to solve it.

There is a .gr2 importer for Blender 2.7x, but it doesn't provide with SWTOR-like materials: it only imports the objects. Still, with some effort, an approximation to the materials of the modern version could be built for 2.7x' Cycles renderer.

<<<<<<< HEAD
=======


>>>>>>> 37df7574dd3f34fa1e7f53f5b87c30dd90724227
## Modding

## Datamining

## Resources

## Getting Help
