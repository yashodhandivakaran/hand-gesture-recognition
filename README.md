#Hello World.
Arun and Michael
Kinect project. Hand gesture recognition. Data visualization. We would like to use color gloves for generating training data.

#[Wiki]

#[Experiment result]

##Vertical mode:
  In vertical mode, the hands are very close to background, not sure if the depth features are good enough.

##Color labeling problem:
  There always seems to exist some noise the mapped depth image. Need understand why. Is depth image already unstable or is the problem of mapping.
  To evaluate the mapped labeling, need to seperate the two issues: mapping of depth->image, and color labeling.

##Tricks
  When using minimum distance for color labeling, cache is used to dramatically improve look-up time. Creadits go to Arun!

###Simple Statistics
   In a single frame with horrizontal mode, there are 300K pixeles, 10K of them may be hands, 77K of them may have -1 of depth.
   A image (sampled 4000 pixel) can generate a LIBSVM format feature vector of size 56MB (each pixel has 2000 features). This is a large number.
[Experiment result]: https://github.com/arunganesan/hand-gesture-recognition/wiki/Experimental-Results

[Wiki]: https://github.com/arunganesan/hand-gesture-recognition/wiki
