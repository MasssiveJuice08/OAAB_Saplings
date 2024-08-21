![OAAB Saplings banner image](https://github.com/MasssiveJuice08/OAAB_Saplings/blob/main/SaplingsTransparent.png)

## Description:  

This mod places saplings from OAAB_Data in most regions on Vvardenfell. 
  
As of version 2.0.0, compatibility is now built-in to run the mod as groundcover in OpenMW. The mod is now an ESM so is made easier to patch, and includes a number of patches for BCOM and other popular mod.
  
## Requirements:  

This mod is a complete replacer for OAAB Saplings and includes the sapling meshes from OAAB Data, now placed in a 'meshes/grass' folder. 

- The original OAAB Saplings mod is not required.  
- If using the '01 patch for OAAB Saplings West Gash for BCOM and SWP', 'Beautiful Cities of Morrowind' and 'Stonewood Pass Reworked' by RandomPal are required.  
- The original 'OAAB Saplings West Gash for BCOM and SWP' patch is not required.  
- 'Melchior's Excellent Grazelands Acacia patch', 'SM Bitter Coast Tree Replacer patch' and 'Graht Morrowind Swamp Trees patch'

## Patches

Packaged with this mod are patches (primarily for BCOM) for the following mods:

**Plugins**
- [BCOM](https://www.nexusmods.com/morrowind/mods/49231)
- [The Stonewood Pass Reworked](https://www.nexusmods.com/morrowind/mods/49464) - requires original mod, BCOM and OAAB_Saplings BCOM patch
- [BCOM Patch for Concept Arts Plantations](https://www.nexusmods.com/morrowind/mods/49231) - requires original mod, BCOM and OAAB_Saplings BCOM patch
- [The Great Seawall of Vivec](https://www.nexusmods.com/morrowind/mods/53544)
- [The Road to the Lighthouse](https://www.nexusmods.com/morrowind/mods/54076)

**Tree Replacers**
- [Graht Morrowind Swamp Trees](https://www.nexusmods.com/morrowind/mods/49771) (not compatible with SM Bitter Coast Tree Replacer patch)
- [Melchior's Excellent Grazelands Acacia](https://www.nexusmods.com/morrowind/mods/51058)
- [SM Bitter Coast Tree Replacer](https://www.nexusmods.com/morrowind/mods/49883) (not compatible with Graht Morrowind Swamp Trees patch)
  
## Installation:  

Pick from the following folders (only `00 Core` is required)

```
- 00 Core (required)
- 01 BCOM Patch (optional)
- 02 The Stonewood Pass patch (optional) - requires BCOM, original mod and 01 BCOM Patch
- 03 BCOM Concept Art Plantations Patch (optional) - requires BCOM, original mod and 01 BCOM Patch
- 04 Great Seawall of Vivec patch (optional)
- 05 The Road to the Lighthouse patch (optional)
- 10 OpenMW Groundcover Patch (optional) - if wanting to run mod as groundcover in OpenMW
- 11 Tree Replacer patches (OpenMW)
   - 01 Melchior's Excellent Grazelands Acacia patch
   - 02 Graht Morrowind Swamp Trees patch
   - 02 SM Bitter Coast Tree Replacer patch (only pick Graht Morrowind Swamp Trees OR SM Bitter Coast Tree Replacer)
- 12 Region Removers (optional) - allows you to optionally remove all saplings from a particular region (pick any)
```
  
### ENABLING GROUNDCOVER IN OPENMW (optional):  

1. Ensure Groundcover is enabled in OpenMW:

 Locate your 'Settings.cfg' folder in your operating system's User Directory:  
- Windows `C:\Users\ *Username* \Documents\my games\OpenMW`  
- GNU/Linux `~/.config/openmw/`  
- OS X `~/Library/Application Support/openmw/`

Add the following lines to the Settings.cfg:  
  
```
[Groundcover]  
enabled = true  
density = 1.0  
min chunk size = 0.5  
stomp mode = 2
stomp intensity = 0
```

- Use either **stomp intensity = '0' or '1'** - using stomp intensity 2 causes the meshes to respond wildly to the player colliding with them.  
  
2) Enable the desired groundcover plugins (DO NOT ACTIVATE THESE IN THE OPENMW LAUNCHER):

- Locate your openmw.cfg (in the same directory as settings.cfg) and add the following lines to the bottom of the document below the last `content=`:  

```
groundcover=OAAB_Saplings_AC.esp  
groundcover=OAAB_Saplings_AI.esp  
groundcover=OAAB_Saplings_BC.esp  
groundcover=OAAB_Saplings_GL.esp  
groundcover=OAAB_Saplings_SG.esp  
groundcover=OAAB_Saplings_WG.esp  
```

**References:**
- [Tips: Performance](https://modding-openmw.com/tips/performance/) (Modding-OpenMW.com) 
- [Groundcover Settings](https://elsid-openmw.readthedocs.io/en/latest/reference/modding/settings/groundcover.html) (OpenMW manual on Read the Docs) 
  
## Acknowledgements:   

- **MelchiorDahrk** and **XeroFoxx** for [Graht Morrowind Swamp Trees](https://www.nexusmods.com/morrowind/mods/49771)  
- **Greatness7** and **Sector** for assistance with using Tes3cmd and Tes3conv.  
  
Make sure to endorse the original mods!
