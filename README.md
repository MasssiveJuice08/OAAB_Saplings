![OAAB Saplings image](https://raw.githubusercontent.com/MasssiveJuice08/OAAB_Saplings/main/SaplingsTransparent.png)

## Description:  

This mod places saplings from OAAB_Data in most regions on Vvardenfell. 
  
**Features as of version 2.0.0:**

- OpenMW groundcover support is now built-in. 
- Core mod is now an ESM so patching is now made easy. 
- Now included are a number of patches for BCOM and other popular mods.
- Optional region remover plugins - if you want to run OAAB Saplings but don't want saplings to appear in a particular region.
- All plugins have been run through [The Lawnmower](https://www.nexusmods.com/morrowind/mods/53034), reducing the reference count by deleting saplings which were hidden beneath buildings and other objects.  
  
## Requirements:  

- [OAAB_Data](https://www.nexusmods.com/morrowind/mods/49042)

The core mod only requires OAAB_Data. However, ensure you have the pre-requisite mods for any patches contained with this mod.

## Patches

Packaged with this mod are patches (primarily for BCOM) for the following mods:

**Plugins:**
- [BCOM](https://www.nexusmods.com/morrowind/mods/49231)
- [The Stonewood Pass Reworked](https://www.nexusmods.com/morrowind/mods/49464) - requires original mod, BCOM and OAAB_Saplings BCOM patch
- [BCOM Patch for Concept Arts Plantations](https://www.nexusmods.com/morrowind/mods/49231) - requires original mod, BCOM and OAAB_Saplings BCOM patch
- [The Great Seawall of Vivec](https://www.nexusmods.com/morrowind/mods/53544)
- [The Road to the Lighthouse](https://www.nexusmods.com/morrowind/mods/54076)

**Tree Replacers:** (only required for OpenMW groundcover users - The original sapling replacer patches will work for vanilla users or OpenMW users who choose not to run the mod as groundcover)
- [Graht Morrowind Swamp Trees](https://www.nexusmods.com/morrowind/mods/49771) (not compatible with SM Bitter Coast Tree Replacer patch)
- [Melchior's Excellent Grazelands Acacia](https://www.nexusmods.com/morrowind/mods/51058)
- [SM Bitter Coast Tree Replacer](https://www.nexusmods.com/morrowind/mods/49883) (not compatible with Graht Morrowind Swamp Trees patch)
  
## Installation:  

Pick from the following folders (only `00 Core` is required)


`00 Core` (required)  
`01 BCOM Patch` (optional)  
`02 The Stonewood Pass patch` (optional) - requires BCOM, original mod and 01 BCOM Patch  
`03 BCOM Concept Art Plantations Patch` (optional) - requires BCOM, original mod and 01 BCOM Patch  
`04 Great Seawall of Vivec patch` (optional)  
`05 The Road to the Lighthouse patch` (optional)  
`10 OpenMW Groundcover Patch` (optional) - if wanting to run mod as groundcover in OpenMW  
`11 Tree Replacer patches (OpenMW)` (optional) - only required for OpenMW groundcover users  
- `01 Melchior's Excellent Grazelands Acacia patch`
- `02 Graht Morrowind Swamp Trees patch`
- `02 SM Bitter Coast Tree Replacer patch` (only pick Graht Morrowind Swamp Trees OR SM Bitter Coast Tree Replacer)  
`12 Region Removers` (optional) - allows you to optionally remove all saplings from a particular region (pick any)  

  
### Load Order

- Any plugins in `12 Region Removers` must load after **all** other OAAB Saplings plugins.
- `OAAB_Saplings SWP patch.esp` and `OAAB_Saplings Concept Art Plantations BCOM patch.ESP` must both load after `OAAB_Saplings BCOM patch.esp`
- **OpenMW groundcover users only**: `groundcover=OAAB_Saplings.esm` should load before all other OAAB Sapling plugins.

It is recommended you use [Mlox](https://github.com/rfuzzo/mlox/releases) or [Plox](https://www.nexusmods.com/morrowind/mods/54262) to sort your load order. Load order rules for OAAB Saplings are already included in [mlox-rules](https://github.com/DanaePlays/mlox-rules). Alternatively, if you are following a modlist from [MOMW](https://modding-openmw.com/), consult the recommended load order given there (**Note**: MOMW is not yet up to date with the latest release of OAAB Saplings)

### OpenMW Groundcover Support (optional):  

OpenMW users can choose to run OAAB Saplings as groundcover, taking advantage of its grass stomping and swaying animations. To enable this, ensure you load any OAAB Saplings plugins (**including the core ESM**) as `groundcover=` in the `openmw.cfg`. Consult the [MOMW guide for 'Groundcover and Stomping'](https://modding-openmw.com/mods/groundcover-and-stomping/) for how to enable and use groundcover in OpenMW.

**Note**: Due to the large size of sapling meshes compared to your usual groundcover mod's grass meshes, it is recommended you use either **stomp intensity = '0' or '1'**. Using stomp intensity 2 causes the meshes to respond wildly to player collision. Setting the stomp intensity lower does not detract negatively from the visual effect of grass stomping in other groundcover mods.   
  
As with any OpenMW groundcover mod, do not activate the plugins in the OpenMW launcher.

Furthermore, the load order of the plugins still matters when loaded as groundcover. `OAAB_Saplings.esm` must load before all other plugins from OAAB Saplings.

## Credits:   

- **MelchiorDahrk** and **XeroFoxx** for [Graht Morrowind Swamp Trees](https://www.nexusmods.com/morrowind/mods/49771)  
- **Greatness7** and **Sector** for assistance with using Tes3cmd and Tes3conv in creating the patches hosted here
- **AcidZebra** for [The Lawnmower](https://www.nexusmods.com/morrowind/mods/53034)
  
Make sure to endorse the original mods!
