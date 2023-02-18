# EECE-571L-PAZ-pre-processing

For each frame in FrontBody there will be a corresponding row added to the emo_list file. 

Edge case 1 - For those frames where PAZ failed to detect face, the emotion label will be denoted as "noFaceDetected".
Edge case 2 - For those frames where PAZ detected multiple "faces", we keep the largest area and remove all the other smaller areas, assuming that the face box is usually larger than that of a non-face box detected. And then we proceed to label the emotion with this one cropped face.
