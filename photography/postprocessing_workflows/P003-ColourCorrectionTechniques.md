# Description: Color Correction Techniques

### Concepts
* None

### Method 1: Using LEVELS Color Correction Masks
* Click Panel - Layer Panel - New Adjustment Layer - Levels.
* Choose RED color and adjust the slider to discard unused RED area.
* Choose GREEN color and adjust the slider to discard unused GREEN area.
* Choose BLUE color and adjust the slider to discard unused BLUE area.

### Method 2: Using CURVES Color Correction Masks
* Click Panel - Layer Panel - New Adjustment Layer - Curves.
* Choose RED color and adjust the RED curve.
* Choose GREEN color and adjust the GREEN curve.
* Choose BLUE color and adjust the BLUE curve.

### Method 3: Using the Neutral Grey in the Image
* Click Panel - Layer Panel - New Adjustment Layer - Levels.
* Use the neutral grey eyedropper and point it to the grey color in the image. 

### Method 4: Using SIMPLE MATH Along with the Neutral Grey in the Image
[Note] If the method 3 does not work then try this method.
* Click Menu - Window - Info Panel.
* Click Tools - Eyedropper Tool.
* Point to the lightest point on the object and click holding the SHIFT key down.
* Check the info panel and compute the average of the Red, Green and Blue values, say X.
* Click Panel - Layer Panel - New Adjustment Layer - Levels.
* Double click on the white eyedropper and subtract X from Red, Green and Blue values and click OK.
* Now point the white eyedropper to the white color in the image.

### Method 5: Applying Color Corrections To Multiple Images By Copying Color Correction Masks
* Open two or more similar images with similar color problems.
* Apply color correction to one of the images using any of the above methods.
* Click - Menu - Window - Arrangements - Tile All Windows Vertically.
* Drag the color correction mask from the corrected image to other images.
* Further fine tune if required.

### Method 6: Applying Color Corrections To Multiple Images Using Droplets
* Click Menu - Window - Actions.
* Click on Panel - Action Panel - Create a new Folder, say "Personal Actions".
* Click on Panel - Action Panel - Create a new Action, say "Color Correction 001".
* Click on Panel - Action Panel - Click on Start Record button.
* Open an image and apply color correction to it using any of the methods 1-4, say using Curves.
* Click on Panel - Action Panel - Click on Stop Record button.
* Click Menu - File - Automate - Create Droplet.
* Fill all the options on the pop up appropriately and click OK.
    - TODO: Expand this.
* This will create a droplet action on the desktop or wherever it is specified.
* Drag an image or a folder containing many images on this shortcut to apply "Color Correction 001" to all the images. 

### Method 7: Match Colors Between Photographs
* Click - Menu - Window - Arrangements - Tile All Windows Vertically.
* Click the first image in the tiled window where the adjustment has to be applied.
* Click - Menu - Image - Adjustments - Match Color.
* Enter source as the second image in the pop up and the correction will be applied instantly. 
* Further fine tune the image by adjusting the Luminance, Color Intensity etc.

### Method 8: Color Corrections For One Particular Object in the Image
* Open an image.
* Click Panel - Layer Panel - New Adjustment Layer - Levels.
* This creates a new adjustment layer and a layer mask.
* Click Tools - Gradient Tool.
* Set Options for Gradient Tool as follows
    - as White/Black
    - as Linear
    - as Normal
    - Opacity as 100%
* Alt-Click on the layer mask to
* ###TODO

### Method 9: Adding a Fill Flash
* Open an image.
* Make a selection using any [Selection techniques](P000a-SelectionTechniques.md).
* Click Mode - Blend Mode
* Click on Blend Mode - Multiply to make it darker.

### Notes
* None

### TODO
* None
