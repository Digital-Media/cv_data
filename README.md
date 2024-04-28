# Data for Courses at the Digital-Media department

This repo contains datasets that can be used for teaching.
At the moment, it contains images/datasets mostly used for Computer Vision lectures.

# Dataset(s)

## Drone Image Pairs (Thermal and RGB)

The `thermal-rgb` folder and corresponding zip-files contain image pairs of thermal and RGB images recorded by a drone.

You can use the scenes `ellipse, FH3, forest`, and `hut` and are well suited for various tasks:

- `ellipse` [:arrow_down: (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_ellipse.zip?raw=true): scene showing the FH's ellipse. Drone was hovering and only rotating around the up-axis. Perfect for panorama stitching.
- `FH3` [:arrow_down: (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_FH3.zip?raw=true): scene showing the FH's FH3 building. Drone was flying at a horizontal distance of around 60m to the building. Suitable for panorama stitching.
- `forest` [:arrow_down: (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_forest.zip?raw=true): scene showing a forest. Drone was flying 50m above the ground. There is no overlap between the images, so panorama stitching is not possible.
- `hut` [:arrow_down: (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_hut.zip?raw=true): scene showing a hut in a zoo. Drone was flying in circular movements around the front of the hut. Might be suitable for panorama stitching (but will be hard).

An exemplary pair of the `ellipse` scene is shown in the following table.
| Thermal | RGB |
| :-: | :-: |
| ![thermal_01](/thermal-rgb/ellipse/T_frame0012.png "a thermal image") | ![rgb_01](/thermal-rgb/ellipse/W_frame0012.png "an RGB image") |

## Hybrid Images

The `hybrid_images` folder and zip-file contains data for creating hybrid images.
The dataset is taken from a [computer vision course at Georgia Tech](https://dellaert.github.io/19F-4476/proj1.html) and features pairs of aligned images.

An exemplary pair is shown in the following table.
| Image A | Image B |
| :-: | :-: |
| ![a motorcyle](/hybrid_images/2a_motorcycle.bmp "a motorcylce") | ![a bike](/hybrid_images/2b_bicycle.bmp "a bike") |

:arrow_down: To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/hybrid_images.zip?raw=true)

## Binary Leaves

The `binary_leaves` folder and .zip-file contais 282 binary images of 5 different leave types.
The binary images are taken from the [Flavia leave dataset](https://flavia.sourceforge.net/) and feature a resolution of $170 \times 128$ pixels. The dataset is intended for binary image processing.
Exemplary images are shown below.

|                   Japanese maple                   |                   Chinese cinnamon                    |                   ginkgo, maidenhair tree                    |                   Chinese tulip tree                    |                   tangerine                    |
| :------------------------------------------------: | :---------------------------------------------------: | :----------------------------------------------------------: | :-----------------------------------------------------: | :--------------------------------------------: |
| ![a Japanes maple leave](/binary_leaves/0/000.png) | ![a Chinese cinnamon leave](/binary_leaves/1/000.png) | ![a ginkgo, maidenhair tree leave](/binary_leaves/2/000.png) | ![a Chinese tulip tree leave](/binary_leaves/3/000.png) | ![a tangerine leave](/binary_leaves/4/000.png) |
|                     56 images                      |                       55 images                       |                          62 images                           |                        53 images                        |                   56 images                    |

:arrow_down: To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/binary_leaves.zip?raw=true)

## Panorama Stitching Images

The `panorama_stitching` folder and .zip-file contains images that can be used for panorama stitching algorithms.
Various images from different sources are included.
| Image(s) | Description, Source (Copyright) |
| :-: | :- |
| ![a panorama](/panorama_stitching/campus_hagenberg.jpg) (1250 x 442) | This image is a panorama image of the campus Hagenberg showing the ellipse, FH1 and FH2. The image can be, for example, cropped in multiple regions and than stitched together. Source: Originally the image was hosted at the Website of the University. Sadly it is offline, now. This version was downloaded form [an alternative: talente-ooe.at](https://www.talente-ooe.at/fileadmin/_processed_/b/0/csm_fhooe-hagenberg-panorama-michael-fruehmann_53e7c4fbb7.jpg) |
| ![imageA](/panorama_stitching/UTA_foto1A.jpg) ![imageB](/panorama_stitching/UTA_foto1B.jpg) (1024x683)| Two images (A and B) recorded at the [University of Texas at Austin](https://en.wikipedia.org/wiki/University_of_Texas_at_Austin). The big tower in image B shows the Main Building. Source: the images are downloaded from the staff website of [Hélio Pedrini](https://www.ic.unicamp.br/~helio/imagens_registro/). |

# Download

In a Jupyter notebook (on Windows and Linux) you can use the following lines of code to download and unzip the entire zip-file of a dataset:

```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/<dataset>.zip" --silent
import zipfile
with zipfile.ZipFile("<dataset>.zip", 'r') as zip_ref:
    zip_ref.extractall(".")
```

Replace `<dataset>` with `hybrid_images`, `binary_leaves` or any other dataset you want to download.
