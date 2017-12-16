# Description: Techniques to Remove Unwanted Objects

### Method 1: Using Clone Stamp Tool
* Create a new layer for non-destructive editing.
    - Click Panels - Layers - New Layer - Rename layer it to 'Remove Object'. 
* Click Tools - Clone Stamp Tool.
* Set Options for clone stamp tool as follows
    - Mode: Normal
    - Opacity: 100%
    - Flow: 100%
    - Aligned Sample: Checked
    - [Important] Aligned Sample Drop Downs: Current & Below or All Layers
* Remove object
    - Use [ or ] to increase or decrease the size of the clone stamp tool.
    - Re-sample Image: Use Alt + Click to select the area of the photo to be used as source.
    - Press down the mouse button on the are where the object has to be removed and drag.
    - [Important] Keep re-sampling image using Alt + Click to avoid any discerning patterns.
* Decrease the opacity of the layer to show a portion of the below layer to give a natural look.
    - Click Panels - Select 'Remove Object' layer - Change the Fill value from 100% to a lower value.

### Method 2: Using Content-Aware Fill
* Select the photo layer. 
* Make a generous selection using any of the selection techniques around the object to be removed. Lasso tool is quite apt for this kind of selection.
* Menu - Edit - Fill - Use should be set to 'Content-Aware' - Click OK.
* This method might create some discerning patterns. Use the clone stamp tool method to remove these patterns.

### Notes
* None

### TODO
* None
