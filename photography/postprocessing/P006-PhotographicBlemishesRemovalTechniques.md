# Description: Techniques to Remove Photographic Blemishes

### Method 1: Using the Clone Stamp Tool
* Use the Method 1: Using Clone Stamp Tool described in [Unwanted Object Removal Techniques](postprocessing/P005-UnwantedObjectsRemovalTechniques.md).
* Use a very small size brush to remove blemishes.

### Method 2: Using the Healing Brush Tool
* Create a new layer for non-destructive editing.
    - Click Panels - Layers - New Layer - Rename layer it to 'Remove Blemishes'. 
* Click Tools - Healing Brush Tool - Healing Brush Tool.
* Set Options for healing brush tool as follows
    - Mode: Normal
    - Source: Sampled checkbox selected.
    - Aligned Sample: Checked
    - [Important] Aligned Sample Drop Downs: Current & Below or All Layers
* Use a very small size brush and apply healings to photographic blemishes.
    - Sample Pattern: Use Alt + Click to get the pattern information from an area of the photo to be used for healing.
      Unlike clone tool, only the pattern information is sampled and not the image area as in clone tool.
    - Click on the spots that needs to be healed.    

### Method 3: Using the Spot Healing Brush Tool
* Create a new layer for non-destructive editing.
    - Click Panels - Layers - New Layer - Rename layer it to 'Remove Blemishes'. 
* Click Tools - Healing Brush Tool - Spot Healing Brush Tool. Note the SPOT healing brush instead of the plain healing 
  brush tool.
* Set Options for healing brush tool as follows
    - Mode: Normal
    - Type: Content-Aware
    - Sample All Layers: Checked
* Use a brush of small size or a size matching the blemish size and keep clicking on the blemishes to remove it.
    - Photoshop uses the pattern info and the color info from the area around the spots and heals the clicked spots.
    - This technique is based on the assumption that the info required to heal a spot is available around the spot. 

### Notes
* Sometime images, especially scanned images, exhibit blemishes on the main subject itself. These are not the unwanted 
  objects in the image but small imperfections on the images itself. The techniques described here should be applied to 
  such cases.

### TODO
* None
