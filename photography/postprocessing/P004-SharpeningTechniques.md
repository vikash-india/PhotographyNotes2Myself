# Description: Image Sharpening Techniques

### Method 1: Using Smart Sharpen Filter
* Change the image to 16-Bit so that there are more information to work with.
    - Menu - Image - Mode - 16-bits/channel.
* Convert background layer to simple layer
    - Double click background layer - Click OK.
* Sharpen the image
    - Menu - Filter - Sharpen - Smart Sharpen
        - Set Preview to selected.
        - Set Basic to checked.
        - Set Setting to default.
        - Adjust the amount to set the contrast of the edges.
        - Adjust the radius to set the pixel on either side of the edges. 
        - Adjust Remove dropdown to Lens Blur.
* Note
    - This might not work with most of the out of focus images.

### Method 2: Using the Lab Color Space
* Change the image to 16-Bit so that there are more information to work with.
    - Menu - Image - Mode - 16-bits/channel or Lab Color.
* Change the color space from RGB to Lab Color.
    - Menu - Image - Mode - Lab Color.
* Select the Lightness channel from Lab/Lightness/a/b.
    - Panel - Channel - Lightness.
* Sharpen the image
    - Menu - Filter - Sharpen - Smart Sharpen
        - Set Preview to selected.
        - Set Basic to checked.
        - Set Setting to default.
        - Adjust the amount to around 121 or as the case may be.
        - Adjust the radius to around 4 or as the case may be. 
        - Adjust Remove dropdown to Lens Blur.
* Select the Lab channel from Lab/Lightness/a/b to bring back the color.
    - Panel - Channel - Lab.
* Change the color space from Lab Color to RGB.
    - Menu - Image - Mode - RGB.
* Now check the final difference using the history panel.

### Method 3: Using Unsharp Mask
* Duplicate the layer to work on the image duplicate.
* Change the image to 16-Bit so that there are more information to work with.
    - Menu - Image - Mode - 16-bits/channel or Lab Color.
* Sharpen the image
    - Menu - Filter - Sharpen - Unsharp Mask
        - Set the amount and Radius like previous methods.
        - Set Threshold to 0 to sharpen everything or set Threshold to 4 to sharpen just a portion of things.

### Method 4 [BEST]: Using High Pass Filter
* Duplicate the layer to work on the image duplicate.
* Change the image to 16-Bit so that there are more information to work with.
    - Menu - Image - Mode - 16-bits/channel or Lab Color.
* Set the blending mode to Overlay.
* Sharpen the image
    - Menu - Filter - Other - High Pass
        - Set the radius to 3.5 or 4.0 and not to a high value.
* If needed copy the overlay layer to create another layer on top over existing overlay layer. 
* Adjust the opacity of the image based on one's personal taste.

### Notes
* Method 4 is better than Method 3 is better than Method 2 is better than Method 1.

### TODO
- None
