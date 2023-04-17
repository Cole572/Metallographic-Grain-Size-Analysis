# Metallographic-Grain-Size-Analysis
Jupyter notebook compatible Python code used to measure grain size in metallurgical micrographs.

The repository contains a metallurgical micrograph of example grains which are imported into the Python code. The methodology for image analysis to measure the grains is: (1) remove noise and improve grain boundary contrast, (2) threshold out the grain boundaries, (3) perform watershed segmentation to isolate each grain as an object, and (4) count the grains by their longest diameter and plot a histogram.

Much of the issue with properly using this method occurs in the thresholding and watershed stage. If there is sufficient noise and a lack of grain boundary contrast, the watershed method will have difficulty parsing between each grain. Also, grains can be split into smaller sections during the watershed, so the correct parameters must be chosen. I've uploaded this file so that others can help me improve it and use it as well.

Thanks!
