Simple-SSD-Stereo
=================

This little script is for anyone interested in the basics of writing stereo-matching code. It's a (very) simple implementation of a sum of squared differences (SSD), support-window based stereo-matching algorithm.

It takes a left and right image (that have to be the same size) and outputs a depth (disparity) map.

Sample left:

![ScreenShot](https://raw.github.com/davechristian/Simple-SSD-Stereo/master/bowling_small_l.png)

Sample right:

![ScreenShot](https://raw.github.com/davechristian/Simple-SSD-Stereo/master/bowling_small_r.png)

Resulting depth map (with 8x8 pixel support window):

![ScreenShot](https://raw.github.com/davechristian/Simple-SSD-Stereo/master/depth.png)

It's not particularly fast (seriously.. you'll need to go make a cup of tea or something), but my aim was to experiment with the actual technique rather than make the fastest Python code evar. The bowling ball test images provided with this code are from the Middlebury stereo dataset 2006<sup>[1]</sup>.

The Python code depends on Numpy (http://www.numpy.org), Matplotlib (http://matplotlib.org) and PIL (http://www.pythonware.com/products/pil), and is licensed under the MIT license (http://opensource.org/licenses/MIT). This version of the code is written for Python 2.7 and I intend to check it with earlier versions and add Python 3.x compatibility soon.

References
----------
[1] H. Hirschmüller and D. Scharstein. Evaluation of cost functions for stereo matching.
In IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR 2007), Minneapolis, MN, June 2007
