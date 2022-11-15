# Data for Courses at the Digital-Media department

This repo contains datasets that can be used for teaching. 
At the moment, it contains images used for Computer Vision lectures.

# Dataset(s)
## Hybrid Images
The `hybrid_images` folder and zip-file contains data for creating hybrid images. 
The dataset is taken from a [computer vision course at Georgia Tech](https://dellaert.github.io/19F-4476/proj1.html) and features pairs of aligned images. 

An examplary pair is shown in the follwoing table. 
|  Image A |  Image B  |
| :-: | :-: |
| ![a motorcyle](/hybrid_images/2a_motorcycle.bmp "a motorcylce") | ![a bike](/hybrid_images/2b_bicycle.bmp "a bike") |

:arrow_down: To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/hybrid_images.zip?raw=true)

In a Jupyter notebook (on Windows and Linux) you can use the following lines of code to download and unzip the hybrid images:
```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/hybrid_images.zip" --silent
import zipfile
with zipfile.ZipFile("hybrid_images.zip", 'r') as zip_ref:
    zip_ref.extractall(".")
```

# Binary Leaves
The `binary_leaves` folder and .zip-file contais 282 binary images of 5 different leave types. 
The binary images are taken from the [Flavia leave dataset](https://flavia.sourceforge.net/) and feature a resolution of $170 \times 128$ pixels. The dataset is intended for binary image processing.
Exemplary images are shown below. 

|  Japanese maple |  Chinese cinnamon  | ginkgo, maidenhair tree | Chinese tulip tree | tangerine |
| :-: | :-: | :-: | :-: | :-: |
| ![a Japanes maple leave](/binary_leaves/0/000.png) | ![a Chinese cinnamon leave](/binary_leaves/1/000.png) | ![a ginkgo, maidenhair tree leave](/binary_leaves/2/000.png) | ![a Chinese tulip tree leave](/binary_leaves/3/000.png) | ![a tangerine leave](/binary_leaves/4/000.png) |
| 56 images | 55 images | 62 images | 53 images | 56 images |

:arrow_down: To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/binary_leaves.zip?raw=true)

In a Jupyter notebook (on Windows and Linux) you can use the following lines of code to download and unzip the hybrid images:
```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/binary_leaves.zip" --silent
import zipfile
with zipfile.ZipFile("binary_leaves.zip", 'r') as zip_ref:
    zip_ref.extractall(".")
```
