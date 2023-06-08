# Panorama-stitching-OPENCV
An OpenCV panorama image Stitcher using image descriptors &amp; keypoints 

This project uses algorithms such as (DoG, Harris etc.) to identify Keypoints & algorithms such as SIFT, SURF etc. to detect local invariant descriptors from the two images. 
Then the descriptors of the two images are matched. 

After this, The RANSAC(Random Sample Consensus) algorithm is used to estimate the homography matrix using our feature vectors. 

Finally, a warping transformation is applied using the homography matrix obtained from the pervious step to finally get the seamless stitched panorama image.  
