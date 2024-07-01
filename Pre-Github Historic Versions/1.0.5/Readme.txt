OAAB Saplings OpenMW Groundcover Patch (OpenMW only)

----------------------------------

DESCRIPTION:
This patch enables OpenMW to utilise Melchior Dahrk's 'OAAB Saplings' as groundcover in OpenMW versions 0.47+, improving engine performance as opposed to the static models.
This is no longer possible with the original OAAB Saplings mod since OpenMW's handling of groundcover changed in OpenMW 0.47.

ALTERNATIVES:
The tools 'Groundcoverizer' by Benjamin Winger and Habasi by Alvazir can create groundcover from all the grass-type flora for your whole load order, reducing the likelihood of conflicts and giving more comprehensive performance improvements. They require a bit of work to get your head around but the payoff is worth is - consider using those instead of this :)
----------------------------------

REQUIREMENTS:
This mod is a complete replacer for OAAB Saplings and includes the sapling meshes from OAAB Data, now placed in a 'meshes/grass' folder.
The original OAAB Saplings mod is not required.

If using the '01 patch for OAAB Saplings West Gash for BCOM and SWP', 'Beautiful Cities of Morrowind' and 'Stonewood Pass Reworked' by RandomPal are required.
The original 'OAAB Saplings West Gash for BCOM and SWP' patch is not required.
02 & 03 folders are OAAB Saplings patches for various tree replacers and require the original mods for the textures.

----------------------------------

INSTALLATION
00 Core - Required. Contains saplings meshes stored in a grass folder, and the six OAAB Sapling ESPs. (Do not enable OAAB_Saplings_WG.esp if using the patch below)
01 Patch for 'OAAB Saplings West Gash for BCOM and SWP' - Optional replacer for the original patch by Mrovkogon's.
02 OAAB_Saplings_AC BCOM Patch - fixes floaters around Sadrith Mora (credit to Sophie)
03 Melchior's Excellent Grazelands Acacia patch - Optional - requires original mod. Load after 00 Core.
04 - Only use one:
	04 Graht Morrowind Swamp Trees patch - Optional - requires original mod. Load after 00 Core.
	04 SM Bitter Coast Tree Replacer patch - Optional - requires original mod. Load after 00 Core. 

----------------------------------

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
stomp intensity = either '0' or '1'

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

----------------------------------

HOW WAS THIS MADE?
OpenMW groundcover mods need to load meshes from a folder called 'Grass'. I just placed the meshes there and changed the file path to the meshes in the plugins.

----------------------------------

ACKNOWLEDGEMENTS: 
Melchior Dahrk as author of OAAB Saplings Mod (https://www.nexusmods.com/morrowind/mods/50334), Melchior's Excellent Grazelands Acacia and Vanilla Friendly West Gash Tree Replacer.
Mrovkogon as author of the original patch 'OAAB Saplings West Gash for BCOM and SWP' - https://www.nexusmods.com/morrowind/mods/50626?tab=files
Melchior Dahrk and XeroFoxx for Graht Morrowind Swamp Trees
CMAugust on the OpenMW Discord for identifying why the original OAAB Saplings no longer worked as groundcover in OpenMW
Greatness7 as author of the Tes3conv tool, used in creating this patch
Hemaris for inspiring this idea with their 'Turn Normal Grass and Kelp into Groundcover' and 'Stirk Performance Improver' mods.
The team at OAAB_Data
Thanks to Sophie on MMC Discord for making the OAAB_Saplings_AC BCOM patch

Make sure to endorse the original mods!