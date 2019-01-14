# Description: Sky Post Processing Techniques

### Concepts
* None

### Adjust the Color of the Sky
* Create a selection of sky using Magic Wand tool.
* Create a color balance adjustment layer using the selection.
* Adjust the color balance. 
* Apply Gaussian Blur to smooth out the affect.
    - Use a low value (say .3) to keep it natural.
    
### Add Sky/Cloud From Another Image
* Main Image Layer
    - Select sky using any of the [Selection Techniques](P001-SelectionTechniques.md) on the main image.
    - Save the selection to the Alpha channel.
* Cloud Image Layer
    - Drag another image with better sky/cloud as a new layer on top of the main image layer.
    - Select the cloud image layer in Panels - Layers. 
    - Load the saved selection from alpha channel by clicking Panels - Channels - Ctrl + Click on the Alpha Channel.
    - Selection will appear on the cloud image layer.
    - Add a new layer mask to mask everything except the selection by clicking Panels - Layers - Add a Layer Mask.  
* Adjust the position of the sky/cloud 
    - Delink cloud image layer with its layer mask by clicking on UNLINK icon on the cloud image layer.
    - Drag the position of the sky/cloud to your choice. 

### Notes
* None

### TODO
* None
