# Face_detection

## AIM

To detect human faces and eyes in digital images using Haar Cascade Classifiers, and to evaluate the performance of the detection on different types of images including single person, person wearing glasses, and group photos. The project also aims to analyze the accuracy and limitations of Haar-based face and eye detection techniques.

## Algorithm for Face and Eye Detection

#### I) Load and Display Images

Import necessary libraries for image processing and visualization.

  - Load images in grayscale format:

  - Single person photo

  - Person wearing glasses

  - Group photo

  - Display the images using a visualization tool so the user can see them.

#### II) Load Haar Cascade Classifiers

  - Load the Haar Cascade for face detection.

  - Load the Haar Cascade for eye detection.

  - These are pre-trained XML classifiers provided by OpenCV.

#### III) Face Detection

  - Define a face detection function that takes a grayscale image as input.

  - Copy the input image to avoid modifying the original.

  - Apply the Haar cascade to detect faces in the image.

  - Draw bounding boxes around the detected faces.

  - Return the processed image and the number of faces detected.

#### IV) Eye Detection

  - Define an eye detection function that takes a grayscale image as input.

  - Copy the input image to avoid modifying the original.

  - Apply the Haar cascade to detect eyes in the image.

  - Draw bounding boxes around detected eyes.

  - Return the processed image and the number of eyes detected.

  - Note: Eye detection may fail if the eyes are covered by sunglasses.

#### V) Apply Detection to Images

  - For each image (single, glasses, group):

  - Call the face detection function and record results.

  - Call the eye detection function and record results.

  - Display the processed images showing detected faces and eyes.

  - Optionally, arrange images in a row or column for comparison.

#### VI) Observations and Limitations

  - Single person image: Face and eyes usually detected accurately.

  - Person with glasses: Face detection may work, but eye detection may fail.

  - Group photo: Some faces may be missed, especially small or partially occluded faces.

#### Limitations of Haar-based detection:

  - Works best with frontal faces.

  - Sensitive to occlusion (glasses, hair, masks).

  - Sensitive to lighting conditions.

  - Less accurate for rotated or angled faces.

  - Reflection: Haar cascades are fast and simple but have lower robustness compared to modern DNN-based detectors.

## RESULT:

#### Single Person Image:

  * Face detected successfully.

  * Eyes detected accurately.

#### Person with Glasses:

  * Face detected successfully.

  * Eye detection partially failed due to sunglasses covering the eyes.

#### Group Photo:

  * Multiple faces detected.

  * Some small or partially occluded faces may not be detected.

  * Eye detection may fail for people with glasses or distant faces.
