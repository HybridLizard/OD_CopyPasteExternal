# OD_CopyPasteExternal
Easily copying and pasting of geometry between 3D Applications

# Why ?

Because quite frankly nothing thats this easy exists.  And if you are like me working in environments using
multiple applications, this becomes extremely beneficial.  I opensourced it, in the hope, that there are other
people willing to contributes, in applications that I have either a) not touched, or b) have not as much experience
in to make this even better than it already is.  So if you are willing to contribute, please get in touch with me.

Currently, it uses an always existing temporary directory to store the intermediate custom file on the local machine,
but of course that directory can be changed to live on a dropbox (for online internet sharing with friends), or on a
network server for inter company sharing.  Those are really just some of the possibilies.

# Help ?

If you want to help and contribute, please get in touch with me.  There's XSI, Cinema4D and 3dsMax that still need
to be done, as well as the Houdini Exporter.  So anyone with experience in the SDK on those apps, please take a look.

# General Information:

- Copy To External: will copy the current mesh into memory
- Paste From External: will rebuild the geometry thats in memory

The following applications are supported:

Modo      : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps

Lightwave : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps

Blender   : Vertices / Polygons (incl. Subpatch and SubD)/ WeightMaps / UVMaps / MorphMaps

Maya      : Vertices / Polygons / Weights (via Vertex Normals)

Houdini   : Vertices / Polygons / Weightmaps, UVMaps

Cinema4D  : None (looking for people to contribute)

3dsMax    : None (looking for people to contribute)

XSI		    : None (looking for people to contribute)

# Installation:

### MODO Install (tested 10.01 and higher):

Drag the OD_ModoCopyPasteExternal folder into your kits folder.
Upon Modo start/restart you now have two additional commands:

OD_CopyToExternal & OD_PasteFromExternal

You'll see a Scissors Icon in your Tailbar which includes those commands.

### LIGHTWAVE Install (2015+):

Add the LW_CopyPasteExternal.py via add plugins. 3 Plugins should be added:

in Layout: OD_LayoutPasteFromExternal
in Modeler: OD_LWPasteFromExternal & OD_LWCopyToExternal
Add them to the menus as you please.

### Maya Install

Just install the two scripts as any other plugin.

### Blender Install (tested 2.78c)

Preferences/Addons/Install from File and select the files and click the checkbox.
The plugins are then found under the object menu.

### Houdini Install (tested 15 and higher)

Start Houdini and open the Python SourceScript editor.  Copy/paste the contents
of the python file into that editor and apply the script.  It will create a new geo
node that has a python file attached and should paste the object.  Currently only
paste is working.

# Tutorials & Videos

Steve White has provided a Youtube Video here showing the use between Modo and Lightwave.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=6jKi34irylo
" target="_blank"><img src="http://img.youtube.com/vi/6jKi34irylo/0.jpg"
alt="LW-Modo Usage" width="240" height="180" border="10" /></a>