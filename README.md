# Hand-Pose-Estimation-CNN
Silhouette-based Pose Estimation.  Hand Segmentation using OpenCV

By continuously sampling the skin tone of the face we develop a calibration range that prepares our application for diverse environments. Applying different approximation and maximization functions we can obtain a segmentation mask of the hand which parallels the input format of our convolutional neural net (CNN). We used a fairly simple learning model to reduce processing requirements. Adjusting sensitivity thresholds and continuously sampling allows our application to remain versatile, enabling further implementation with personal devices.

We wagered the open-source computer vision library, OpenCV, to segment frames in order to best align them with the input of the model. We define two skin tones, an upper and lower bound as defined by our faceToSkinTone(FTST) method. The FTST can be used simultaneously with the pose prediction model or separately(recommended) to predefine the user’s average skin tone in a given environment.

After 15 epochs our model reached 83.3% testing accuracy across ten classes.

For further insights into the methodology please read the attached Silhouette-based Pose Estimation driven by Adaptive Hand Segmentation.PDF

Dataset: 
Rooban Sappani. “Hand Gesture Recognition” Kaggle. Retrieved December 2021
  From https://www.kaggle.com/roobansappani/hand-gesture-recognition. 2021.
