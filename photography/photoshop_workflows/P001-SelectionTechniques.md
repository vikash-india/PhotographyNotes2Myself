# Description: Selection Techniques

### Concepts
* There are many techniques to create a selection.
* Multiple selection techniques can be combined to create a single selection.
* Sometime it's easier to select the opposite of what needs to be selected. Then invert the selection by clicking 
  Menu - Select - Inverse Selection.
* There are common operations applicable to a selection irrespective of the selection technique used. 
* Adjust Selections
    - Use Shift to add to a selection. 
    - Use Alt to subtract from a selection.
    - Use Shift and Alt together to get an intersection of the selection.
* Create a new layer from the selection 
    - Copying Selection: Menu - Layer - Layer via Copy
    - Cutting Selection: Menu - Layer - Layer via Cut
* Create a new adjustment layer after making a selection
    - Panels - Layers - New Adjustment Layer.
    - This will add a Layer Mask along with the Adjustment Layer.
* Complex selections can be saved for easy recall and reuse.
    - The selections are saved as new channels in Panel - Channels. 
    - Save selection by clicking Panels - Channels - Save Selection as Channel. This will create a new Alpha channel 
      under Panel - Channels. 
    - Selection can ALSO be saved by clicking Menu - Selection - Save Selection. This will create a channel with custom 
      name provided.
    - Once the selection is saved, use Tools - Brush Tool - Brush Tool to remove or add from the saved selection by 
      painting over the selection using white or black.
* Soften the selection edges using any of the techniques. 
    - Use Gaussian Blur to soften the edges.  
        - Click on the layer mask. 
        - Click Menu - Filter - Blur - Gaussian Blur.
        - Adjust the values. 
* Refine Edges
    - Make selection using any of the methods below. 
    - Click on Menu - Select - Refine Edges.
    - Set Options for Refine Edges
        - View: Change to black
        - Smooth: 0-3
        - Feather: 0.3
        - Contrast: 0
        - Shift Edge: Use the slider to point to the middle.
        - Output: New Layer with Layer Mask 

### Method 1: Selection Using Magical Wand Tool
* Click Tools - Quick Selection Tool - Magic Wand Tool.
* Set Options for Magic Wand Tool
    - Sample-size: Point Sample
        - This value comes from the Eye Dropper Tool. If the value is modified for Eye Dropper Tool, it will get 
          modified here too.
    - Tolerance: 32
        - The default value is 32. It has a range of 0-255.
    - Anti-alias: Checked
    - Contiguous: Checked
        - Uncheck this if the same color should be selected even if they are not contiguous.
    - Sample All Layers: Unchecked
* Click on the image to make a selection.
    - Use Shift or Alt to add to or remove from a selection.
* Use any of the common operations to make the selection more natural. 
    - Use Gaussian Blur to soften the edges.
* Now work with the selection.

### Method 2: Selection Using Quick Selection Tool
* Click Tools - Quick Selection Tool - Quick Selection Tool.
* Set Options for Quick Selection Tool
    - Brush Size: 30
    - Sample All Layers: Unchecked
        - Set it to checked for using with multiple layers.
    - Auto-Enhance: Checked
        - This is used for enhancing the top layer.
* Start dragging to make a selection. 
* Use any of the common operations to make the selection more natural. 
* Now work with the selection.

### Method 3: Selection Using Magnetic Lasso Tool for Detecting Edges
* Click Tools - Lasso Tool - Magnetic Lasso Tool.
* Set Options for Magnetic Lasso Tool
    - Feather: 0
        - Keep this 0 and use Gaussian Blur later on to soften the edges. 
    - Anti-alias: Checked
    - Width: 10
        - Width of 10 means lasso tool will stick within 10 pixels. 
    - Contrast: 10%
    - Frequency: 57
        - Lower frequency means more stops.
        - Higher frequency means less stops.
* Move over the edges of the selection and continue till the starting point.
    - Create manual stops by clicking in case the tool does not detect edges properly. 
    - Use backspace to remove stops created by mistake.
* Use any of the common operations to make the selection more natural. 
* Now work with the selection.

### Method 4: Selections Using Pen Tool for Precise Selections
* Pen tool is used to make straight or curve lines. 
* Click Tools - Pen Tool - Pen Tool.
* Click on each of the corners of the subject to make a selections using straight line selection.
    - Click on the starting point to create a selection. 
    - The selection will be available on a new Layer as well as a path in Panels - Paths. 
* Adjust the selection to make it more precise 
    - Tools - Path Selection Tool - Direct Selection Tool.
    - Click on the corners and adjust the selection or use the arrow keys to adjust the selection.
* Convert the path to Selection
    - Panels - Paths - Load Path as Selection.
* Use any of the common operations to make the selection more natural. 
* Now work with the selection.
    - Now the selection can be converted to an adjustment layer with layer mask and edited.

### Method 5: Selections Using Paint Brush Tool
* Click Tools - Quick Mask Mode
* Double Click on Quick Mask Mode - Set Selected Area as checked. 
* Paint on the image to make a selection. 
    - Use black color to paint the selection.
    - Use white color to remove/subtract from the selection.
* Click on Quick Mask Mode to highlight the selection. 
* Use any of the common operations to make the selection more natural.
* Now work with the selection.

### Method 6: Refining a Channels Selection
* Choose the layer with the subject.
* Click Panel - Channel
    - Channels hold the color information. 
    - The percentage is based on the shades of grey. The darker shade of grey means less of that color. The lighter 
      shade of grey means more that color.  
    - Click on Red, Green and Blue individually to find the channel which gives the maximum contrast.
    - Make a copy of the channel which gives the maximum contrast for non-destructive editing.
    - Select this copy channel.
* Use curve to create contrast 
    - Click Menu - Image - Adjustments - Curves. 
        - Drag the highlights above the curve line.
        - Drag the shadows below the curve line.
        - Click OK
* Use Threshold to split the component to black and white 
    - Click Menu - Image - Adjustments - Threshold. 
    - Use the slider to get more of the subject to be selected and click OK.
    - Threshold splits the components to black and white using the original shades of grey. 
* Use the Brush Tool to clean the mask
    - Click Tools - Brush Tool - Brush Tool.
        - Use White to remove the selection. 
        - Use Black in the inner areas to add to selection.
        - DO NOT disturb the edges.
* Make a final selection
    - Bring back the image by clicking Panels - Channels - Set RGB as checked.
    - Make the selection by clicking Panels - Channels - Ctrl + Click on Copy channel.
    - Use Menu - Select - Inverse Select to select the subject instead of the background.
* Refine the Edges
    - Click on Menu - Select - Refine Edges.
    - Set Options for Refine Edges
        - View: Change to black
        - Edge Detection: Set Smart Radius as Checked.
        - Smooth: 0-3
        - Feather: 0
        - Contrast: 0
        - Shift Edge: Use the slider to point to the middle.
    - Paint around the edges to refine it.
        - Use [ or ] to increase or decrease the brush size. 
    - Change the options for Refine Edges
        - Decontaminate Colors: Checked
            - Slide the amount to make the selection perfect.    
        - Output: New Layer with Layer Mask
        - Click OK
* Use any of the common operations to make the selection more natural. 
* Now work with the selection.
    - [Tip] This method can be used to change the background of the selected subject.   

### Notes
* None

### TODO
* None
