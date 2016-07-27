Fisheye Camera Calibration Set failing fisheye calibration
==========================================================

This repository contains a set of calibration images, that fail calibibration using
[opencvs camera_calibration tutorial app][https://github.com/opencv/opencv/tree/master/doc/tutorials/calib3d/camera_calibration].
from [opencv-master][https://github.com/opencv/opencv/commit/9ad0dcb57fca5cb0fd66e2854854942d5b286e43] branch.

The images where taken with a GoPro Hero3+ black. The calibration app is
configured to used opencvs fisheye camera model. Write extrinsics is disabled,
as this feature currently crashes.


Call for camera_calibration app:

    $CV_BINS_PATH/cpp-tutorial-camera_calibration config-fisheye.xml

The results are not plausible. Especially distortion coefficients are all zero.
See the results in [this file](out_camera_fisheye_data.xml).
