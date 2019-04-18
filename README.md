# Interactive-Region-Growing-Segmentation
This is an interactive region growing algorithm which will take in user seeds and segment the region from the image. The segmented result can be improved by adding additional seeds and guiding the algorithm

<p align="center">
  <img src="https://github.com/SamarthGupta93/Interactive-Region-Growing-Segmentation/blob/master/Brain_ct_8.png" title="Brain Tumor Segmentation">
  <img src="https://github.com/SamarthGupta93/Interactive-Region-Growing-Segmentation/blob/master/Brain_ct_15.png" title="Brain Cerebrum Segmentation">
</p>


### Region Growing algorithm 
➢ Interactive algorithm which will allow you to input one or more seed points using the left mouse click

➢ Segmentation can be improved by providing additional seed points on the segmented result 

### Settings
Threshold – 10 (This was found to be the best value for a fast segmentation with good results) 

Neighbors - (1,0), (0,1), (-1,0), (0,-1) (4 Neighbors. Left, Right, Up and Down) 

Note: You can also try with 8 neighbors (this contains the 8 pixels around a given pixel). The command is provided below in the “Working” section.

### Working 
Run the program using the command (4 neighbours): 

➢ python region_growing.py --image_path image_path 

To run with 8 neighbours, use this command:  
➢ python region_growing.py --image_path image_path --conn 8 

### Program Steps
1. Convert the image provided into grayscale image and ask for user seeds 
2. Provide one or more user seeds by clicking the left mouse button. Once done, press any key to start the segmentation 
3. Wait for few seconds for the segmentation process to complete and the results will be displayed 
4. You can input additional seeds on the display by clicking the left mouse button to improve the segmentation results 

**Save** the result – To Save the segmented result, press “s”. 
**Exit** – Press “Esc” to exit from the segmentation (only works when you are on the segmentation display screen) 

Feel free to try on images of any size. Resizing will be done if the image size is too big
