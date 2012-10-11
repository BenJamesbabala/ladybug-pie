Project: ladybug-pie
====================
Author: Jay W Johnson

Description:
Python wrapper for Ladybug3 Spherical Camera API.

Only the methods that handle pre-recorded *.pgr files have been wrapped. Methods for controlling the camera and recording video have not been wrapped. The software that comes with the camera is good enough for recording video.

***
### Ladybug package
**interface.py**
* Ladybug3stream class

    Simplifies management of a *.pgr stream file and adds additional methods not included in the Ladybug API.

**API.py**
* LadybugAPI class

    Access to pythonified ladybug.dll methods.
    Memory management tasks are handled by the class.
    Data written by the method are returned by the method instead of returning an error code.

***
### SFM package
**opticflow.py**
* FeatureMatcher class

    Implements OpenCV's FeatureDetector_create, Descriptor_create, and flann_index methods to do feature detection and matching over a series of images.
    
    TODO: Still needs some testing and clean-up and the addition of a bundle adjustment method.




