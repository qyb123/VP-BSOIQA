# VP-BSOIQA
VP-BSOIQA metric release.

========================================================================

-----------COPYRIGHT NOTICE STARTS WITH THIS LINE------------
Copyright (c) 2020 The Ningbo University
All rights reserved.

Permission is hereby granted, without written agreement and without license or royalty fees, to use, copy, 
modify, and distribute this code (the source files) and its documentation for
any purpose, provided that the copyright notice in its entirety appear in all copies of this code, and the 
original source of this code, Multi-media Signal Processing Laboratory at the Ningbo University
, is acknowledged in any publication that reports research using this code. The research
is to be cited in the bibliography as:

1) Y. Qi, G. Jiang, M. Yu, Y. Zhang, and Y.-S. Ho, "VP-BSOIQA Metric Release", 
URL: https://codeload.github.com/qyb123/VP-BSOIQA/zip/master, 2020

2) Y. Qi, G. Jiang, M. Yu, Y. Zhang, and Y.-S. Ho,"Viewport Perception based Blind Stereoscopic Omnidirectional Image Quality Assessment", 
IEEE Transactions on Circuits and Systems for Video Technology, in review.

IN NO EVENT SHALL THE NINGBO UNIVERSITY BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, 
OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OF THIS DATABASE AND ITS DOCUMENTATION, EVEN IF THE NINGBO UNIVERSITY 
HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

THE NINGBO UNIVERSITY SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED 
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE DATABASE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS,
AND THE NINGBO UNIVERSITY HAS NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.

-----------COPYRIGHT NOTICE ENDS WITH THIS LINE------------%

Author  : Yubin Qi 
Version : 1.0

The authors are with the Laboratory for Multi-media Signal Processing
, Department of Electronic and Communication Engineering, The
Ningbo University, Ningbo, China.

Kindly report any suggestions or corrections to qiyubin123@126.com

========================================================================

This is a demonstration of the Viewport Perception based Blind Stereoscopic 
Omnidirectional Image Quality Assessment (VP-BSOIQA) method.
The algorithm is described in:

Y. Qi, G. Jiang, M. Yu, Y. Zhang, and Y.-S. Ho,"Viewport Perception based Blind Stereoscopic Omnidirectional Image Quality Assessment", 
IEEE Transactions on Circuits and Systems for Video Technology, in review.

You can change this program as you like and use it anywhere, but please
refer to its original source (cite our paper and our web page at
https://codeload.github.com/qyb123/VP-BSOIQA/zip/master).

========================================================================

Running on Matlab 


Input : A test image and corresponding saliency map loaded in an array

Output: A set of perceptual features (a total of 240 dimension).
  
Usage:

1. Run demo.m

2. Dependencies: 

Subfunction files:  provided with release in the "util" file.

Image Files: d_img.png, s_img.png, ts_img.png

Toolbox： tensor_toolbox

========================================================================
Note on Image Files: 

d_img.png: The distorted stereoscopic omnidirectional image
s_img.png:  The calculated left and right saliency map
ts_img.png: The calculated binocular combination saliency map

Here, the saliency detection algorithm designed for stereoscopic images is
used to form the "s_img.png", and run the TensorImg.m to form the "ts_img.png".

Ref: W. Wang, J. Shen, Y. Yu, and K. Ma, “Stereoscopic thumbnail creation
via efficient stereo saliency detection,” IEEE Trans. Vis. Comput.
Graph., vol. 23, no. 8, pp. 2014-2027, Aug. 2017.

========================================================================

