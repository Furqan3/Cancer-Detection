# Skin Lesion Classification using Image Processing and Machine Learning
This project aims to classify skin lesions into two categories: normal and melanoma. The classification is based on four features extracted from images of skin lesions using image processing techniques. The four features are asymmetry, border, color, and diameter.

### Features
![image](https://user-images.githubusercontent.com/88136810/233147528-5d05ac30-e289-48c4-b82c-1de3462ad65d.png)

- #### Asymmetry
Asymmetry is a measure of the difference in shape between the left and right halves of a skin lesion. The feature is calculated by dividing the lesion into four quadrants, and then computing the entropy of the pixel intensity distribution in each quadrant.

- #### Border
Border is a measure of the irregularity of the border of a skin lesion. The feature is calculated by eroding the grayscale image of the lesion and then computing the circularity of the difference between the original grayscale image and the eroded image.

- #### Color
Color is a measure of the variation in color of a skin lesion. The feature is calculated by converting the lesion image to the YUV color space and then computing the standard deviation of the mean Y, U, and V values of the lesion.

- #### Diameter
Diameter is a measure of the size of a skin lesion. The feature is calculated by finding the maximum and minimum pixel values in the lesion image, and then computing the Euclidean distance between these points.

### Dataset
The dataset used for this project is the PH2 Dataset, which consists of 200 skin lesion images. The dataset is divided into two classes: normal and melanoma.

Usage
The `main.py` file contains the implementation of the feature extraction and classification pipeline. To run the pipeline, simply run the following command:

```
python main.py
```
The pipeline first extracts the four features from the images in the dataset, and then uses a random forest classifier to classify the images into normal or melanoma. The classification results are then printed to the console.

### Dependencies
The following libraries are required to run the code:
```
numpy
pandas
matplotlib
opencv-python
```
You can install these dependencies using pip:
```
pip install numpy pandas matplotlib opencv-python
```
### Results
The classification results achieved by the pipeline are as follows:
```
Accuracy: 0.83
```
### Features Extracted
- #### Box PLot
![image](https://user-images.githubusercontent.com/88136810/233146693-50e2894f-878e-4a3b-b751-2fd796ba84df.png)
- #### Histogram Plot
![image](https://user-images.githubusercontent.com/88136810/233146814-7a099878-0e63-4659-a2ff-f6afe8c22966.png)

- #### Scater Plot
![image](https://user-images.githubusercontent.com/88136810/233146903-b4bd9e5a-eb1a-47ba-8149-ce8240c41c8f.png)

### Feature Data
![image](https://user-images.githubusercontent.com/88136810/233147382-b86f1931-3044-40d9-a01d-c62f91c64575.png)
 ### Accuracy
![image](https://user-images.githubusercontent.com/88136810/233147450-a6083e4e-f218-4111-be86-f10386ec0ea0.png)


