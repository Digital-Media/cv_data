# Data for Courses at the Digital-Media department

This repo contains datasets that can be used for teaching.
At the moment, it contains images/datasets mostly used for Computer Vision lectures.

# Dataset(s)

## Drone Image Pairs (Thermal and RGB)

The `thermal-rgb` folder and corresponding zip-files contain image pairs of thermal and RGB images recorded by a drone.

You can use the scenes `ellipse, FH3, forest`, and `hut` and are well suited for various tasks:

- `ellipse` [⬇️ (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_ellipse.zip?raw=true): scene showing the FH's ellipse. Drone was hovering and only rotating around the up-axis. Perfect for panorama stitching.
- `FH3` [⬇️ (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_FH3.zip?raw=true): scene showing the FH's FH3 building. Drone was flying at a horizontal distance of around 60m to the building. Suitable for panorama stitching.
- `forest` [⬇️ (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_forest.zip?raw=true): scene showing a forest. Drone was flying 50m above the ground. There is no overlap between the images, so panorama stitching is not possible.
- `hut` [⬇️ (direct download)](https://github.com/Digital-Media/cv_data/blob/main/thermal-rgb_hut.zip?raw=true): scene showing a hut in a zoo. Drone was flying in circular movements around the front of the hut. Might be suitable for panorama stitching (but will be hard).

An exemplary pair of the `ellipse` scene is shown in the following table.

|                                Thermal                                |                              RGB                               |
| :-------------------------------------------------------------------: | :------------------------------------------------------------: |
| ![thermal_01](/thermal-rgb/ellipse/T_frame0012.png "a thermal image") | ![rgb_01](/thermal-rgb/ellipse/W_frame0012.png "an RGB image") |

## Hybrid Images

The `hybrid_images` folder and zip-file contains data for creating hybrid images.
The dataset is taken from a [computer vision course at Georgia Tech](https://dellaert.github.io/19F-4476/proj1.html) and features pairs of aligned images.

An exemplary pair is shown in the following table.

|                             Image A                             |                      Image B                      |
| :-------------------------------------------------------------: | :-----------------------------------------------: |
| ![a motorcyle](/hybrid_images/2a_motorcycle.bmp "a motorcylce") | ![a bike](/hybrid_images/2b_bicycle.bmp "a bike") |

⬇️ To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/hybrid_images.zip?raw=true)

## Binary Leaves

The `binary_leaves` folder and .zip-file contais 282 binary images of 5 different leave types.
The binary images are taken from the [Flavia leave dataset](https://flavia.sourceforge.net/) and feature a resolution of $170 \times 128$ pixels. The dataset is intended for binary image processing.
Exemplary images are shown below.

|                   Japanese maple                   |                   Chinese cinnamon                    |                   ginkgo, maidenhair tree                    |                   Chinese tulip tree                    |                   tangerine                    |
| :------------------------------------------------: | :---------------------------------------------------: | :----------------------------------------------------------: | :-----------------------------------------------------: | :--------------------------------------------: |
| ![a Japanes maple leave](/binary_leaves/0/000.png) | ![a Chinese cinnamon leave](/binary_leaves/1/000.png) | ![a ginkgo, maidenhair tree leave](/binary_leaves/2/000.png) | ![a Chinese tulip tree leave](/binary_leaves/3/000.png) | ![a tangerine leave](/binary_leaves/4/000.png) |
|                     56 images                      |                       55 images                       |                          62 images                           |                        53 images                        |                   56 images                    |

⬇️ To directly download a zip folder of the dataset use [this link!](https://github.com/Digital-Media/cv_data/blob/main/binary_leaves.zip?raw=true)

## Panorama Stitching Images

The `panorama_stitching` folder and .zip-file contains images that can be used for panorama stitching algorithms.
Various images from different sources are included.

|                                                Image(s)                                                | Description, Source (Copyright)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| :----------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|                  ![a panorama](/panorama_stitching/campus_hagenberg.jpg) (1250 x 442)                  | This image is a panorama image of the campus Hagenberg showing the ellipse, FH1 and FH2. The image can be, for example, cropped in multiple regions and than stitched together. Source: Originally the image was hosted at the Website of the University. Sadly it is offline, now. This version was downloaded form[an alternative: talente-ooe.at](https://www.talente-ooe.at/fileadmin/_processed_/b/0/csm_fhooe-hagenberg-panorama-michael-fruehmann_53e7c4fbb7.jpg) |
| ![imageA](/panorama_stitching/UTA_foto1A.jpg) ![imageB](/panorama_stitching/UTA_foto1B.jpg) (1024x683) | Two images (A and B) recorded at the[University of Texas at Austin](https://en.wikipedia.org/wiki/University_of_Texas_at_Austin). The big tower in image B shows the Main Building. Source: the images are downloaded from the staff website of [Hélio Pedrini](https://www.ic.unicamp.br/~helio/imagens_registro/).                                                                                                                                                     |

## Exemplary Images (for various tasks)

The `example_images` folder contains exemplary images that can be used for various tasks.

|                   Image                   | Description, Source                                                                                                                                                                                                                   |
| :---------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|      ![cat](/example_images/cat.jpg)      | A cute cat image. Source:[Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Cat03.jpg/481px-Cat03.jpg)                                                                                                     |
|     ![gogh](/example_images/gogh.jpg)     | An image of a painting by Vincent van Gogh. Source:[Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Vincent_van_Gogh_-_National_Gallery_of_Art.JPG/367px-Vincent_van_Gogh_-_National_Gallery_of_Art.JPG) |
| ![einstein](/example_images/einstein.jpg) | An image of Albert Einstein. Source:[The Laboratory for Computational Vision is an interdisciplinary research group at New York University](https://www.cns.nyu.edu/~lcv/ssim/index_files/image003.jpg)                               |
|    ![woman](/example_images/woman.jpg)    | An image of a woman. Useful for showcasing edge and line detection. Source:[Flickr](https://live.staticflickr.com/8859/18045025168_3a1ffa6521_c_d.jpg)                                                                                |
|   ![sudoku](/example_images/sudoku.png)   | An image of a sudoku puzzle. Useful for thresholding algorithms. Source:[OpenCV](https://raw.githubusercontent.com/opencv/opencv/4.x/samples/data/sudoku.png)                                                                         |

## Object Detection Sample Images

The `object_detection` folder contains a small set of multi-object scenes used to demo modern detectors (YOLO, RT-DETR) and Vision-Language Models (e.g. Gemma 4). The classes shown — *person*, *car*, *bus*, *apple*, *banana*, *orange* — are all part of the COCO-80 label set, so pretrained detectors work out of the box.

|                          Image                           | Description, Source                                                                                                                                                                                                                                                                            |
| :------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    ![fruits](/object_detection/fruits.jpg) (1264 x 848)   | A wooden bowl on a wooden table containing whole apples, bananas, and oranges — for vision-language detection (e.g. *"detect: apple, banana, orange"*) and open-vocabulary queries like *"the leftmost fruit"*. Source: synthetic, generated with Google's Gemini 3 Pro Image. |

## Structure From Motion (SFM) Example Images (for various tasks)

The `SFM` folder contains images that can be used for Structure From Motion (SFM).
In the subfolders you can find images of different scenes that can be used for SFM tasks.

- `Ellipse` [⬇️ (direct download of images as zip)](https://github.com/Digital-Media/cv_data/blob/main/SFM/Ellipse/input.zip?raw=true): scene showing the FH's ellipse. Images show a drone flight with 3 different heights and angles. Images are extracted from a video and subsampled. Note that the matching of the images is not perfect for all images.

An exemplary set of images is shown in the following table.

|                  Image 00                   |                  Image 33                   |                  Image 99                   |
| :-----------------------------------------: | :-----------------------------------------: | :-----------------------------------------: |
| ![ellipse_01](/SFM/Ellipse/input/00000.jpg) | ![ellipse_02](/SFM/Ellipse/input/00033.jpg) | ![ellipse_02](/SFM/Ellipse/input/00099.jpg) |

## Tiny NeRF Data

The file `tiny_nerf_data.npz` is the dataset used by the [`11b_TinyNeRF.ipynb`](https://github.com/Digital-Media/vco/blob/vco2025/11b_TinyNeRF.ipynb) tutorial — a small, self-contained Neural Radiance Field (NeRF) demo. It contains **106 views** (100 × 100 RGB images), the corresponding **4 × 4 camera poses**, and the **focal length** (≈138.89), all in a single NumPy `.npz` archive.

Originally sourced from Ben Mildenhall & Matthew Tancik's [`tiny_nerf.ipynb`](https://github.com/bmild/nerf/blob/master/tiny_nerf.ipynb) (`cseweb.ucsd.edu/~viscomp/projects/LF/papers/ECCV20/nerf/tiny_nerf_data.npz`); mirrored here for reliability.

⬇️ Direct link: [`tiny_nerf_data.npz`](https://github.com/Digital-Media/cv_data/blob/main/tiny_nerf_data.npz?raw=true)

```python
import numpy as np
data = np.load("tiny_nerf_data.npz")
images, poses, focal = data["images"], data["poses"], data["focal"]
print(images.shape, poses.shape, float(focal))
# (106, 100, 100, 3) (106, 4, 4) 138.8888788992210
```

## FH HGB Hockey Dataset

The `fhhgb-hockey-dataset.zip` contains a hockey-related dataset recorded at / for FH Upper Austria Hagenberg, used in computer vision exercises (e.g. detection / tracking on hockey footage). See the dataset author for the exact contents, splits, and licence.

⬇️ Direct link: [`fhhgb-hockey-dataset.zip`](https://github.com/Digital-Media/cv_data/blob/main/fhhgb-hockey-dataset.zip?raw=true)

# Download

In a Jupyter notebook (on Windows and Linux) you can use the following lines of code to download and unzip the entire zip-file of a dataset:

```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/<dataset>.zip" --silent
import zipfile
with zipfile.ZipFile("<dataset>.zip", 'r') as zip_ref:
    zip_ref.extractall(".")
```

Replace `<dataset>` with `hybrid_images`, `binary_leaves`, `thermal-rgb_ellipse`, `thermal-rgb_FH3`, `thermal-rgb_forest`, `thermal-rgb_hut`, or `fhhgb-hockey-dataset`.

For loose files (no zip needed) just `curl` or `wget` them directly, e.g.:

```python
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/tiny_nerf_data.npz" --silent
!curl -LJO "https://raw.githubusercontent.com/Digital-Media/cv_data/main/object_detection/street.jpg" --silent
```
