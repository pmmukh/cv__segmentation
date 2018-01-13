# cv__segmentation
Segmentation

The code performs semi-automatic binary segmentation based on SLIC superpixels and graph-cuts using the following steps:
1. Given an image and sparse markings for foreground and background
2. Calculate SLIC over image
3. Calculate color histograms for all superpixels
4. Calculate color histograms for FG and BG
5. Construct a graph that takes into account superpixel-to-superpixel interaction (smoothness term), as well as superpixel-FG/BG interaction (match term)
6. Run a graph-cut algorithm to get the final segmentation
