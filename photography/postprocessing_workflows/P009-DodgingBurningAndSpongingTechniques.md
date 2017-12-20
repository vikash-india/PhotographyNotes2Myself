# Description: Dodging, Burning and Sponging Techniques

### Concepts
* Dodging is a technique to lighten up an area of an image. 
* Burning is a technique to darken an area of an image. 
* Sponging is a technique to increase or decrease the saturation of colors in an area of an image. 
* Dodging, burning and sponging should ONLY be used for enhancing a selective area of an image and NOT the whole image.
* It is possible to use dodging in one area of an image and burning on another area of the same image.
* Dodging, burning and sponging are concepts and can be applied without using the dodge and burn tools. Method 5 and 6 
  are such examples of dodging and burning without using the dodge and burn tools. 

### Method 1: Lighten up an area using Dodge Tool
* Duplicate the layer for non-destructive editing.
* Click Tools - Dodge Tool - Dodge Tool.
* Set the options for the dodge tool as follows
    - Range: Midtones
        - Start with midtones even when working on Shadow areas.
    - Exposure: 40%. 
        - This value decide how aggressive is the dodge tool.
        - Start with a value of 25%-40% and find a comfort zone for each image.
    - Enable Air Brush Style Build-up Effects: Off
        - Turn this on if working on a tablet with pressure pen.
        - This uses pressure to control the size of the brush and the exposure.  
    - Protect Tone: Checked
        - Protect the tones as the image is dodged.
    - Always Use Pressure for Size: Off
        - Turn this on if working on a tablet with pressure pen.
        - This uses titling of the brush to get a different brush size.
* Choose appropriate brush size and rub on an area of an image to lighten it up. 
    - Use [ or ] to increase of decrease the brush size. 
    - Keep adjusting the size of the brush to match the area size of the image. 
    - Do not overlap an area otherwise it will lightened up more. 
    - Rubbing on an area multiple times lightens the image multiple times.
    - Use the same speed to rub an area.
*  Fix an area lightened up by mistake.
    - Sometime dodging and burning might cross the desired area and lighten an already highlighted area or further 
      darken an area which is already in the shadow. 
    - Create a new layer.
    - Click Tools - History Brush Tool - History Brush Tool.
        - Paint back the area of image as it was in the original by rubbing it on the affected area.
        - Being generous with the painting wont do any harm as history brush does not change things which has not been 
          modified.  
    - Modify the layer opacity to control the amount of dodging. 

### Method 2: Darken an area using Burn Tool
* Duplicate the layer for non-destructive editing.
* Click Tools - Dodge Tool - Burn Tool.
* Set the options for the burn tool just like in Method 1.
    - Range: Midtones
    - Exposure: 40%. 
    - Enable Air Brush Style Build-up Effects: Off
    - Protect Tone: Checked
    - Always Use Pressure for Size: Off
* Choose appropriate brush size and rub on the area of an image to darken it.
    - Same rules of dodge tool described in method 1 applies to burn tool as well.
     
### Method 3: Dodging, Burning and Sponging Using the Quick Mask Selection Tool
* Duplicate the layer for non-destructive editing.
* Click Tools - Quick Mask Tool
    - This tool is used to paint a selection.
* Click Tools - Brush Tool - Brush Tool. 
    - Choose paint color as black.
* Set the options for the Brush Tool as below
    - Hardness: 0
        - This will result in a soft brush.
* Paint over an area of the image that should be selected.
    - Use [ or ] to increase of decrease the brush size. 
    - Choose paint color as white to correct an area painted by mistake.
    - This technique will not create a hard area. 
* Click Menu - Filter - Blur - Gaussian Blur
    - This is an optional step to further soften the blur. 
    - Use a start value of 50% and adjust up or down.  
* Click Tools - Quick Mask Tool again to convert the painted area into a selection.
    - Use Ctrl+H to toggle the visibility of the selection.  
    - Check if the selection should to be inverted to get a desired selection. 
* Use either the dodge tool from method 1 to lighten the selected area
    - This step could flatten the color of the area too. 
* Use sponging to bring back the color.
    - Click Tools - Dodge Tool - Sponge Tool. 
    - Set the options for the sponge tool as follows
        - Mode: Saturate (To add colors)
        - Flow: 25%
            - This is to set how fast it works.
            - Start with 25% and find the appropriate levels. 
        - Vibrance: Checked
        - Leave other option values to their default values.
* Alternatively, one can use the burn tool from method 2 to darken the selected area and use the sponge tool with mode 
  as Desaturate to remove the colors.

### Method 4: Dodging and Burning Using Custom Brushes
* Duplicate the layer for non-destructive editing.
* Click Tools - Dodge Tool - Burn Tool.
* Set the options for the burn tool just like in Method 1.
    - Range: Midtones
    - Exposure: 40%. 
    - Enable Air Brush Style Build-up Effects: Off
    - Protect Tone: Checked
    - Always Use Pressure for Size: Off
* Click on the Toggle the Brush Panel from the options for the Burn Tool.
    - This will open a pop up.
    - Change the roundness to create a custom brush size to match the object, say a water stream width.
    - Change the angle to make the brush perpendicular to the object, say water stream.  
    - Change the spacing to give a natural effect to the brush.

### Method 5: Dodging and Burning Using Layer Masks
* Duplicate the layer for non-destructive editing.
* Use any of the [Selection Techniques](P000a-SelectionTechniques.md) to make a selection from an image that needs 
  dodging and burning.
* Click Panel - Layer Panel - New Adjustment Layer - Exposure.
    - This will create an exposure adjustment layer with selection highlighted in white and other area in black.
    - Adjustment to exposure will only affect the white area leaving the black area of the image unchanged.
    - This technique should be used when a large portion of an image needs a correction. 
    - Dodging and burning can be applied without using the dodge and burn tool.    
* Click on the Adjustments panel and increase the exposure to lighten up the area or decrease the exposure to darken the 
  area.
* Use any of the [Color Balancing Techniques](P003a-ColorBalancingTechniques.md) to balance the colors if required. 

### Method 6: Dodging and Burning Using Layer Blending Modes
* Duplicate the layer for non-destructive editing.
* Click Panels - Layers - Select Screen from the Layer Blending Modes dropdown.
    - The Screen mode is used to lighten up the layer.
    - The Multiple mode is used to darken up the layer. 
    - Layers with blending mode can be duplicated to apply the blending modes multiple times and increase the effect. 
* The blending mode applies to whole layer. Use layer mask to apply the changes to only a portion of the image.
    - Choose the layer on which the Screen Blending Mode has been applied. 
    - Make a selection on the image layer.
    - Create a layer mask by clicking Panels - Layer Panel - Add Vector Mask (Layer Mask). 
        - Now the Screen mode only applies to the white area in the layer mask.
* Duplicate this layer with layer mask to increase the effect of blending modes. Adjust the opacity of the layer to 
  control 
    
### Notes
* None

### TODO
* None
