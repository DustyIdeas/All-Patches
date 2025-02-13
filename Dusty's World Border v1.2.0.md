# **Patch Notes** -  12/7/24 @ 6:28 AM PT

## **Updates**
- **Updated for Minecraft Bedrock version `1.21.50.7`.**  
  *Note:* This version is not compatible with earlier releases.

---

## **Changes**
- **Adjusted `BORDER_PROXIMITY`** from **15 blocks** to **30 blocks** for improved gameplay experience.  

- **Reworked the custom command `#br`:**  
  It is now a **tag-based system**, allowing you to assign tags to players to initiate border movement.  
  Examples:  
  - Move the border from a radius of 10 to 15 over 10 seconds:  
    `/tag @r add _br_10_15_10`  
  - Stop border movement:  
    `/tag @r add _br_stop`

---

## **Added**
- **New Toggle for End/Nether 1:8 Border Ratio**  
  Accessible via the GUI menu, this option is enabled by default.

- **Border Radius and Damage Customization via Tags:**  
  Use tag prefixes to modify the border settings:  
  - Change radius: `/tag @r add _br_radius_<NUMBER>`  
  - Change damage: `/tag @r add _br_damage_<NUMBER>`  
    *Note:* Damage values:  
    - `1` = half a heart  
    - `0` = disables damage

---

## **Fixes**
- **Resolved crash when transitioning between dimensions:**  
  Transitioning from the Nether/End to the Overworld no longer causes crashes.  
  *Issue Details:* This occurred when a portal spawned the player beyond the border due to the End/Nether's 1:8 block ratio.  
  *Note:* This issue may persist for players on low-end devices (e.g., mobile or low-spec PCs).

- **Texture Fix in GUI: Fixed an issue where the custom textures used inside the GUI were being displayed as the default textures for the items.**
