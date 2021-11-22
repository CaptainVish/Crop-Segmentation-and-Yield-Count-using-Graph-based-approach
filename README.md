# Crop-Segmentation-and-Yield-Count-using-Graph-based-approach

Implemented code for semi-automatic binary segmentation based on SLIC superpixels and graph-cuts.Image Segmentation is dividing an image into meaningful non overlapping regions, according to some objective criterion, homogeneity in some feature space or separability in some other. It eliminates unwanted background and produce the foreground image of the nuts making the counting of clustered nuts easier.

The analysation of natural images and estimating the total count available is an important task in computer vision applications. Arecanut images are natural images, and analysis of these images plays an important role in the Indian market. To count the areca visual descriptors of an image are used. There are several automated techniques available for other fruits and crops, but no technique is available for identifying the arecanuts in bunches before harvesting. Thus, such an identification system is needed.

# Static Segmentation:

For static segmentation, user needs to pass a mask of same size as of image with foreground and background markings. Foreground marking should be in Red color and Background makrings should be in Blue color. Run the following command to execute the segmentation:

> python staticSegmentation.py [original image Path] [marking image Path] [output directory ex. ./]

# Dynamic Segmenttaion:

For run time segmentation, an interactive window will popup. User can draw markings on the image. Red color represents the marking for Foreground and Blue colors represents the markings for Background. Once, atleast one marking is available for FG and BG, corresponding result will pop up in another window showing the binary mask. Mask is updated in real time as a line is drawn by the user.
By default Foreground mode is set. Use following keys to interact with window:

'f' - switch to Foreground mode

'b' - switch to Background mode

'r' - Reset markings

'q' - Quit

Python command:

> python interactiveSegmentation.py  [original image Path]

Refer [Real Time Segmentation](https://github.com/techiepanda/Image-segmentation-using-SLIC-superpixels-and-graph-cuts/blob/master/Real%20Time%20Segmentation.mov) to see the working example.

