# Data for Courses at the Digital-Media department

This repo contains datasets that can be used for teaching. 
At the moment, it contains images used for Computer Vision lectures.

# Dataset(s)
## Hybrid Images
The `hybrid_images` folder and zip-file contains data for creating hybrid images. 
The dataset is taken from a [computer vision course at Georgia Tech](https://dellaert.github.io/19F-4476/proj1.html) and features pairs of aligned images. 

An examplary pair is shown below
|  Image A |  Image B  |
| ----------------------------------------------------------------|---------------------------------------------------|
| ![a motorcyle](/hybrid_images/2a_motorcycle.bmp "a motorcylce") | ![a bike](/hybrid_images/2b_bicycle.bmp "a bike") |

To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/hybrid_images.zip?raw=true)

In a Jupyter notebook (on Windows and Linux) you can use the following lines of code to download and unzip the hybrid images:
```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/hybrid_images.zip" --silent
import zipfile
with zipfile.ZipFile("hybrid_images.zip", 'r') as zip_ref:
    zip_ref.extractall(".")
```
