OAAB Saplings OpenMW Groundcover Patch (OpenMW only)

DESCRIPTION:
This patch enables OpenMW to utilise Melchior Dahrk's 'OAAB Saplings' as groundcover in OpenMW versions 0.47+, improving engine performance as opposed to the static models.
This is no longer possible with the original OAAB Saplings mod since OpenMW's handling of groundcover changed in OpenMW 0.47.

WHY USE THIS MOD:
Converting non-container flora (e.g. vanilla Ash Grass, as opposed to Trama Root which is a container) models into groundcover is a great way to improve performance in OpenMW.
I got the idea originally from Hemaris and his 'Turn Normal Grass and Kelp into Groundcover' mod.
Pros: Improved performance, as well as utilising OpenMW's swaying animation (groundcover sways gently in the breeze)
Cons: The saplings meshes are not optimised for OpenMW's grass stomping animation - try to walk through it and the mesh will greatly stretch and distort until you are far away again. 
The above can be negated by turning off 'grass stomping' in the settings.cfg (but I just ignore it, personally).

REQUIREMENTS:
This mod is a complete replacer for OAAB Saplings and includes the sapling meshes from OAAB Data, now placed in a 'meshes/grass' folder.
The original OAAB Saplings mod is not required (nor is OAAB Data itself, technically)
If using the '01 patch for OAAB Saplings West Gash for BCOM and SWP', 'Beautiful Cities of Morrowind' and 'Stonewood Pass Reworked' by RandomPal are required.
The original 'OAAB Saplings West Gash for BCOM and SWP' patch is not required.
02, 03, 04 and 05 folders are OAAB Saplings patches for various tree replacers and require the original mods for the textures.

INSTALLATION
00 Core - Required. Contains saplings meshes stored in a grass folder, and the six OAAB Sapling ESPs. (Do not enable OAAB_Saplings_WG.esp if using the patch below)
01 patch for 'OAAB Saplings West Gash for BCOM and SWP' - Optional replacer for the original patch by Mrovkogon's.
02 Melchior's Excellent Grazelands Acacia patch - Optional - requires original mod. Load after 00 Core.
03 Vanilla Friendly West Gash Tree Replacer patch - Optional - requires original mod. Load after 00 Core and 01 OAAB Saplings West Gash for BCOM and SWP.
04 SM Bitter Coast Tree Replacer patch - Optional - requires original mod. Load after 00 Core. 
05 Graht Morrowind Swamp Trees patch - Optional - requires original mod. Load after 00 Core.

ENABLING GROUNDCOVER IN OPENMW - REQUIRED:

1) Ensure Groundcover is enabled in OpenMW:
 Locate your 'Settings.cfg' folder in your operating system's User Directory:
- Windows	C:\Users\ *Username* \Documents\my games\OpenMW
- GNU/Linux	~/.config/openmw/
- OS X	~/Library/Application Support/openmw/
Add the following lines to the Settings.cfg:

[Groundcover]
enabled = true
density = 1.0
min chunk size = 0.5
stomp mode = 2
stomp intensity = 2

2) Enable the desired groundcover plugins (DO NOT ACTIVATE THESE IN THE OPENMW LAUNCHER):
Locate your openmw.cfg (in the same directory as settings.cfg).
Add the following lines to the top of the document:

groundcover=OAAB_Saplings_AC.esp
groundcover=OAAB_Saplings_AI.esp
groundcover=OAAB_Saplings_BC.esp
groundcover=OAAB_Saplings_GL.esp
groundcover=OAAB_Saplings_SG.esp
groundcover=OAAB_Saplings_WG.esp [or if using the BCOM SWP patch, replace "OAAB_Saplings_WG.esp" with "OAAB_Saplings_WG-BCoM+SWP.esp"]

More info on groundcover settings in OpenMW can be located here:
https://modding-openmw.com/tips/performance/
https://elsid-openmw.readthedocs.io/en/latest/reference/modding/settings/groundcover.html


HOW WAS THIS MADE?
I moved the original saplings meshes from "meshes/oaab/f" to "meshes/grass". 
In order for the OAAB Saplings ESPs to utilise the meshes in their new location, I had to edit the ESPs.
I did this by converting each esp to a JSON file with tes3conv and added new info instructing it to use the grass meshes in their new locations, eg.,
  {
    "type": "Static",
    "flags": [
      0,
      0
    ],
    "id": "AB_Flora_AcSapling02",
    "mesh": "grass\\ABsaplingAC02.NIF"
  },


ACKNOWLEDGEMENTS: 
Melchior Dahrk as author of OAAB Saplings Mod (https://www.nexusmods.com/morrowind/mods/50334), Melchior's Excellent Grazelands Acacia and Vanilla Friendly West Gash Tree Replacer.
Mrovkogon as author of the original patch 'OAAB Saplings West Gash for BCOM and SWP' - https://www.nexusmods.com/morrowind/mods/50626?tab=files
Melchior Dahrk and XeroFoxx for Graht Morrowind Swamp Trees
CMAugust on the OpenMW Discord for identifying why the original OAAB Saplings no longer worked as groundcover in OpenMW
Greatness7 as author of the Tes3conv tool, used in creating this patch
Hemaris for inspiring this idea with their 'Turn Normal Grass and Kelp into Groundcover' and 'Stirk Performance Improver' mods.
OAAB Team for the Saplings patch for SM Bitter Coast Tree Replacer.

Make sure to endorse the original mods!