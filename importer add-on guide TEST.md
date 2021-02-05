### How to use the .gr2 importer add-on for Blender to assemble and texture SWTOR characters

This is a provisional guide to importing SWTOR characters into Blender, applying preset materials to them, and adjusting such materials.

If you followed older guides based on the use of EasyMYP to extract the game assets and Noesis to convert them into usable formats, be aware that we no longer need such conversions thanks to the Blender import/export addon that understands SWTOR's .gr2 format. Also, there is no longer a need to modify the texture files in Photoshop or similar packages: Blender understands the .dds image format, and the preset materials provided by that same addon do all the required channel manipulations. So, Noesis is no longer necessary, although it still is useful as a model visor and, in certain cases, as a model and texture converter for less capable 3D apps.

Once installed in Blender, the addon shows up as:

![](images/extracting/gr2-addon/gr2_addon_guide_010.png)

Its only importing option is the "Import Collision Mesh" checkbox, which normally will be left unchecked.

#### Assigning SWTOR materials to imported character objects

Let's suppose we have imported the parts of a character. They'll appear correctly positioned already.

![](images/extracting/gr2-addon/gr2_addon_guide_030.png)

![](images/extracting/gr2-addon/gr2_addon_guide_020.png)

<img align="left" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_040.png">

If you happen to switch the Outliner to Blender File mode (no real need, but it is interesting), you'll notice that there are a series of new material "templates": Creature, Eye, Garment, HairC, SkinB, and Uber (they are created by the addon the moment it imports a .gr2 file). Those names match the <derived> label that appears at the heading of the .mat material definition files, which tells us which one we'll use for each object.

You'll notice, too, that some of the materials have names that match the name of the .mat files, but some didn't manage that and defaulted to "default" and the like. That is a current limitation of the importer addon. It's not really a problem because we are going to disregard those materials, replacing them with copies of the templates.

In the Outliner, twirling the objects' little left-side arrows, you can see their meshes and materials (and vertex groups, which aren't relevant for this tutorial).

<img align="right" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_050.png">

You'll see that sometimes there are two materials in an object instead of a single one. That usually happens in three cases:

* • A head that has a skin material and an eyes material.
* • A "hair piece" such as a Zabrak's horn plus hair object, which has materials for the hair and the horns.
* • A piece of armor that shows skin. As SWTOR replaces whole body parts with corresponding pieces of armor, those need to incorporate the skin of the body part they replace, which uses its own material. 

Let's start with, say, the chest part. I've opened a Shader Editor panel which shows that it's been assigned a default material consisting of the usual Principled BSDF shader (Blender defaults to that because it's kind of a Swiss Army knife shader)

![](images/extracting/gr2-addon/gr2_addon_guide_055.png)

We are NOT going to use that default material: what we are going to do is replace it with one of the Template Materials that the addon created in the project at the moment of importing the model. As typical of any bare skin body part (or bit of skin showing in any piece of sexy armor), the .mat file tells us that we have to use a "skinb" shader.

![](images/extracting/gr2-addon/gr2_addon_guide_060.png)

So, with the object selected and the Shader Editor showing its material, we use the materials menu to select the SkinB Shader template. This will result in the replacement of the original material assignment with the SkinB Shader one.

![](images/extracting/gr2-addon/gr2_addon_guide_070.png)

But we need to do something before continuing: yes, the materials are named "template" this and that, but Blender has no template system yet (there is an asset library system doing trials in the latest betas), so we need to make a duplicate to preserve the original. If we don't, we risk finding ourselves rewriting and using the same material in different body parts without meaning to.

For that, we'll simply click on the New Material button next to the Material name in the menu:

![](images/extracting/gr2-addon/gr2_addon_guide_080.png)

As the name field is so narrow, you probably won't see that the name was appended a ".001" or similar. You can check it by opening the selection menu, or by double-clicking the field (the cursor will move to the end of the name, so it will become visible).

![](images/extracting/gr2-addon/gr2_addon_guide_090.png)

Once having assigned this duplicate of the template, it's best that you change that name to something more comprehensible. Say, "Chest".

![](images/extracting/gr2-addon/gr2_addon_guide_100.png)

#### Applying textures and values to the character's materials

Now, let's give the material a look. You can see that there is a big custom node (Node Group, in Blender's parlance) at the right side, and a lot of unassigned texture file nodes, named with the texture file suffixes that belong in each (ending in "_d", "_s", etc.).

![](images/extracting/gr2-addon/gr2_addon_guide_110.png)

Well: the idea is that you click on their "Open" buttons, browse to the correspondingly
suffixed files, and load them.

![](images/extracting/gr2-addon/gr2_addon_guide_120.png)

![](images/extracting/gr2-addon/gr2_addon_guide_130.png)

One thing you'll have to do for each of those, once assigned, is set their Color Space setting to "Raw" (Blender defaults them to sRGB, which isn't appropriate for the way these SWTOR materials work, especially in the case of non-image texture files such as the "_n" normal maps).

![](images/extracting/gr2-addon/gr2_addon_guide_140.png)

The SkinB shader works for the head body part too: that's why it includes nodes for Complexions and FacePaints (tattoos, fur patterns, etc.). The .mat file will tell you what to use in those nodes when it's not a head material: files like "white", "default_facemap", etc.). Currently, the material doesn't support scar or wrinkles maps. We are looking into that.

#### The problem with character's color data

Now that we have all the texture files assigned, we can see about filling the big node group's fields with the data necessary to reproduce the colors and finish of the game's object. Most of it is in the .mat files, and its labelling matches the one in the node, but some of it isn't, most specifically the skin color (which happens to be the most important one, isn't it?). We'll see to it.

<img align="left" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_150.png">

The Palette1's X, Y, Z, and W fields are meant to work very much like Photoshop's (or any other painting app's) Hue Saturation Lightness Adjustment tool. The fields are:

* Palette1.X = Hue adjustment.
* Palette1.Y = Saturation adjustment.
* Palette1.Z = Brightness adjustment.
* Palette1.W = Contrast adjustment.

The thing is: if we can't get the correct values (we can: it's just a bit involved), we can still eyeball them. Set Palette1.Z (brightness) and Palette1.W (contrast) to 0.5 or so to get the skin to a somewhat neutral lightness and then play with them all to try to approximate the skin color you want (use shift-click'n'drag on those fields to change them in fine increments/decrements).

<img align="right" width="250" border-color="white" src="images/extracting/gr2-addon/gr2_addon_guide_160.jpg">

As for the Palette1 Specular and Metallic Specular, the corresponding data in the .mat files comes as value triplets, but you'll notice that in the node there are color wells instead. No trouble: just open them and enter the values as R, G, B (and Alpha if there is a fourth value listed).

Let's see now about getting the exact values for the Palette1 fields.

The problem we have is that, although most of the information about the objects' materials is present in the .xml and .mat files extracted with EasyMYP, there are bits that only exist in the game's nodes database, so we need NodeViewer to consult it (and maybe extract it to have it more at hand).

The skin, eye and hair's colors appear in the dynamic menu's related submenus: inside them, their nodes' names are the filenames that supposedly ought to exist in the EasyMYP extraction but, alas, don't.

![](images/extracting/gr2-addon/gr2_addon_guide_180.png)

For example, in the case of this Zabrak character, I can find the node and see there the Palette information I need. Note that the order of the fields in NodeViewer doesn't match the order in Blender's node, so remember what's what to place the values correctly:

* Palette1.X = appPaletteHue.
* Palette1.Y = appPaletteSaturation.
* Palette1.Z = appPaletteBrightness.
* Palette1.W = appPaletteContrast.

You can find there the Specular and MetallicSpecular values, too.

If a value appears with a minus sign, omit the sign (not yet fully sure about this but it seems to work).

![](images/extracting/gr2-addon/gr2_addon_guide_190.png)

For the material to handle transparency (typical of fine edge detail such as hair strands) while using the Eevee renderer, remember to set both the material's Blend Mode and Shadow Mode to "Alpha Clip". 

![](images/extracting/gr2-addon/gr2_addon_guide_200.png)

And that's it, mostly. We'll be adding to this tutorial to make it more handholding-ish, so any suggestions to improve it are welcome)


Notes:

The current version of the .gr2 importer works in both Blender 2.8x and 2.9x, but the materials of a project started in 2.8x won't fully work in Blender 2.9x without some minor modifications: Blender introduced a new input socket in 2.9x' Principled Shader between the "Emission" and the "Alpha" ones, and that makes some of the materials' shader network "noodles" connect to the wrong inputs. It's easy to correct manually.

There is a .gr2 importer for Blender 2.7x, but it doesn't provide with SWTOR-like materials: it only imports the objects.

We are still looking for the connection between armor gear and the garmenthue nodes of the dynamic block. 



