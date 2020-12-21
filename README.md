# Image-Segmentation-Model

Image segmentation is a critical process in computer vision. It involves dividing a visual input into segments to simplify image analysis. Segments represent objects or parts of objects, and comprise sets of pixels, or “super-pixels”. Image segmentation sorts pixels into larger components, eliminating the need to consider individual pixels as units of observation. There are three levels of image analysis:
* **Classification** – categorizing the entire image into a class such as “people”, “animals”, “outdoors”
* **Object detection** – detecting objects within an image and drawing a rectangle around them, for example, a person or a sheep.
* **Segmentation** – identifying parts of the image and understanding what object they belong to. Segmentation lays the basis for performing object detection and classification.

<p align="center">
    <img alt="Image Segmentation" title="Image Segmentation" src="https://missinglink.ai/wp-content/uploads/2019/03/what-is-image-segmentation-e1553795451244.png">
</p>

In this project I have automated the process of detecting and localizing defects found in Steel manufacturing. Detecting defects would help in improving the quality of manufacturing as well as in reducing the waste due to production defects. The team has collected images of steel surfaces which can be used as training data to develop a model that could detect and localize defects in real-time. 12600 images that contain 4 types of defects, along with their location in the steel surface have been provided.

First, we must classify the image to check whether it has a defect or not. This is done using a ResNet50 model. Once that is done, we take the defect images and pass it through a ResUnet model which will be trained to identify and highlight the defective area.
