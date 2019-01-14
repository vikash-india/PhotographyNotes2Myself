# Description: Selection Techniques

### Concepts
* There are many techniques to create a selection.
* Multiple selection techniques can be combined to create a single selection.
* Sometimes it's easier to select the opposite of what needs to be selected. Then invert the selection by clicking 
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
    - Tips
        - Experiment with the different values of Tolerance.
        - Experiment Click on different points in images to get the desired selection.
        - Apply this method on skies.
    - Sample-size: Point Sample
        - This value comes from the Eye Dropper Tool. Modify the value for Eye Dropper Tool, to modified here too.
        - Although this option affects the Magic Wand tool, it appears on the Options bar only when the Eyedropper tool 
          is selected. The Sample Size value means the following
            - Point Sample: Samples just the color of the pixel clicked.
            - 3 by 3 Average: Averages the color of the pixel clicked and the surrounding eight pixels.
            - 5 by 5 Average: Averages the color of the pixel clicked and the surrounding 24 pixels.
            - 11 by 11 Average: Averages the color of the pixel clicked and the surrounding 120 pixels.
            - 31 by 31 Average: Averages the color of the pixel clicked and the surrounding 960 pixels.
            - 51 by 51 Average: Averages the color of the pixel clicked and the surrounding 2,600 pixels.
            - 101 by 101 Average: Averages the color of the pixel clicked and the surrounding 10,200 pixels.
    - Tolerance: Start with 32.
        - The tolerance has a range of 0-255. The default value is 32.
        - Setting the tolerance to 0 selects one color only.
        - Setting the Tolerance to 255 selects all colors.
        - The default value of 32 means that the Magic Wand tool selects all colors that are 16 levels lighter and 16 
          levels darker than the base color.
        - If the Magic Wand tool selected more than you wanted it to, lower the Tolerance setting. If it didn’t select 
          enough, raise the setting.
    - Anti-alias: Checked
        - Checked: Softens the edge of the selection by one row of pixels.
        - Unchecked: 
    - Contiguous: Checked
        - Checked: Select only pixels that are adjacent to each other. 
        - Unchecked: Selects all pixels within the range of tolerance, whether they’re adjacent to each other or not.
    - Sample All Layers: Unchecked
        - Checked: If there are multiple layers, the Magic Wand selects pixels from all visible layers. 
        - Unchecked: The tool selects pixels from the active layer only.
* Click on the image to make a selection.
    - Use Shift or Alt to add to or remove from a selection.
* Use any of the common operations to make the selection more natural. 
    - Example: Use Gaussian Blur with low values like .3 to soften the edges.
* Now work with the selection.

### Method 2: Selection Using Quick Selection Tool
* Click Tools - Quick Selection Tool - Quick Selection Tool.
* Set Options for Quick Selection Tool
    - Brush Size: 30
        - Experiment with different brush size.
    - Sample All Layers: Unchecked
        - Checked: Makes a selection from all the layers. 
        - Unchecked: select only from the current layer.
    - Auto-Enhance: Checked
        - This is used for enhancing the top layer.
        - Checked: Automatically refine selection by implementing an algorithm.
* Start dragging to make a selection. 
* Use any of the common operations to make the selection more natural. 
* Tips
    - Select the Alpha channel and uncheck R, G, and B channel and paint white to remove unwanted selections. 
* Now work with the selection.

### Method 3: Selection Using Magnetic Lasso Tool for Detecting Edges
* Click Tools - Lasso Tool - Magnetic Lasso Tool.
* Set Options for Magnetic Lasso Tool
    - Feather: 0
        - This value is used to soften the edges. 
        - Keep this 0 and use Gaussian Blur later on to soften the edges later.
    - Anti-alias: Checked
        - Checked: Smoothing of jagged edges in digital images by averaging the colors of the pixels at a boundary.
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
    - Double click on "Work Path" and give appropriate name.
* Adjust the selection to make it more precise 
    - Click Tools - Path Selection Tool - Direct Selection Tool.
    - Click on the corners and adjust the selection or use the arrow keys to adjust the selection.
        - Click on Ctrl + One Corner to make only one corner move.
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

### Method 6: Selection Using Channels Selection
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

### Refine Edges of a Selection
* Main Uses
    - This is often used to refine complex selection like an hair selection.
* Make a Selection
    - Make a selection using any of the above methods.
* Separate the Selection
    - Click on Layers panel - Layer Mask tool to separate the selection.     
* Refine the Edges
    - Click on Menu - Select - Refine Edges.
    - Set Options for Refine Edges
        - View Mode
            - View: Change to black
                - Marching Ants: The selection will be surrounded by marching ants. Keyboard shortcut is M.
                - Overlay: The selection will be overlaid by the layer mask which default color is light red. Keyboard  
                  shortcut is V.
                - On Black: One of the most used mode. In this mode the area that is not selected is filled with black 
                  color. It gives a high contrast so its easy for to select the image. Keyboard shortcut is B.
                - On White: Just opposite of "on black" mode. The area which is not selected will be filled by white  
                  color. Keyboard shortcut is W.
                - Black & White: In this mode the area that is selected will be filled by white color and the area that  
                  is not selected will be filled by black color. Keyboard shortcut is K.
                - On Layers: In this mode the area which is not selected will becomes transparent. Note that one may see 
                  check board pattern. That pattern indicates the transparent layer. Keyboard shortcut is L.
                - Reveal Layer:This mode displays an image without any selection. Keyboard shortcut is R.
            - Show Radium: Unchecked
            - Show Original: Unchecked
        - Edge Detection
            - Box: Select Refine Radius Tool
                - Refine Radius Tool: Refines the selection.
                - Erase Refine Radius Tool: Erases the selection.
            - Smart Radius: Checked.
                - Checked: When checked, Photoshop will decide weather the selection is hard (selection of table, chair)  
                  or soft(hair, fur). 
                - Always turn on this setting every time.
            - Radius: 0
                - Use Radius if Smart Radius is unchecked.
                - This controls the radius of the refine edge tool. Basically it determines how far should the refine 
                  edge tool should go to refine your edge.
        - Adjust Edge
            - Smooth: 0-3
                - It smoothens a selection. 
                - Use it while selecting hair, fur, trees etc.
            - Feather: 0
                - It softens the selection. 
                - It helps a lot when one is creating vignette effect to a photo.
            - Contrast: 0
                - It sharpens an edge even if one softens it by using feather or smoothens it by using smooth.
            - Shift Edge: Use the slider to point to the middle.
                - -100: This shifts the edge away from the selection. This expands a selection.
                - 100: This shifts the edge towards the selection. This contract a selection
        - Output
            - Decontaminate Colors: Checked
                - This option helps reduce edge leftover colored pixels around the edges of a selection that one sees 
                  only after putting the object on a new background. Once this is checked, Photoshop tries to replace 
                  the color of selected pixels with the color of pixels nearby (whether they’re selected or not). 
            - Amount: 
                - Drag the Amount slider to the right to change the color of more edge pixels, or to the left to change 
                  fewer.
            - Output: New Layer with Layer Mask
        - Click OK
    - Paint around the edges to refine it.
        - Use [ or ] to increase or decrease the brush size. 
    - Change the options for Refine Edges
* Now work on the selection. 

### Notes
* None

### TODO
* None
