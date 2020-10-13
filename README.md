# Google-Open-Images-Mutual-Gaze-dataset
This dataset consists of images along with annotations that specify whether two faces in the photo are looking at each other. This dataset is intended to aid researchers working on topics related to social behavior, visual attention, etc.

## Dataset content
The dataset is released as CSV files. Each line in a CSV file corresponds to one data sample, which consists of images and annotations that indicate whether two faces in the photo are looking at each other.

Each image is specified using an image ID/url and two face bounding boxes (top-left and bottom-right coordinates).

The Image URL serves as a preview of the image. Please access the image from [OpenImageV4](https://storage.googleapis.com/openimages/web/download_v4.html) using Image ID if the original image is removed from the public domain.

Each annotation is a boolean from the set {0, 1}. A value of 1 (0) means both faces are (not) looking at each other. 

Each line in the CSV files has the following entries:\
ImageID (string): The image ID in [OpenImageV4](https://storage.googleapis.com/openimages/web/download_v4.html).\
ImageUrl (string): Url of image.\
Annotation (boolean): Human annotation that indicates if both faces are looking at each other.\
XminBoxA (float): Top-left column of the face bounding box A normalized with respect to width.\
YminBoxA (float): Top-left row of the face bounding box A normalized with respect to height.\
XmaxBoxA (float): Bottom-right column of the face bounding box A normalized with respect to width.\
YmaxBoxA (float): Bottom-right row of the face bounding box A normalized with respect to height.\
XminBoxB (float): Top-left column of the face bounding box B normalized with respect to width.\
YminBoxB (float): Top-left row of the face bounding box B normalized with respect to height.\
XmaxBoxB (float): Bottom-right column of the face bounding box B normalized with respect to width.\
YmaxBoxB (float): Bottom-right row of the face bounding box B normalized with respect to height.

## Dataset statistics
This dataset is divided into two partitions:\
Train set (26410 samples):  train_data.csv \
Test set (6659 samples):  test_data

## License
Creative Commons Attribution 4.0 International License ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))

## Contacts
Please email Ching-Hui Chen ([chuichen@google.com](mailto:chuichen@google.com)), Raviteja Vemulapalli ([ravitejavemu@google.com](mailto:ravitejavemu@google.com)) or Yukun Zhu ([yukun@google.com](mailto:yukun@google.com)) for any questions regarding the dataset.

## Acknowledgements
We thank the Intelligent Photography team from Google for their support and suggestions during the data collection process.
