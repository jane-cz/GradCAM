# Grad-CAM
This repo contains 2 implementations of the [Grad-CAM](https://arxiv.org/pdf/1610.02391.pdf) saliency map on the model provided in [this tutorial](https://captum.ai/tutorials/CIFAR_TorchVision_Interpret), on the CIFAR-10 dataset.
* The first implementation was adapted from [this tutorial](https://medium.com/@stepanulyanin/implementing-grad-cam-in-pytorch-ea0937c31e82).
* The second implementation used the [pytorch-grad-cam](https://github.com/jacobgil/pytorch-grad-cam) package.

## Here are some sample results:

| Original image(plane) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(ship1) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(ship2) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(cat) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(car) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/car/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/car/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/car/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/car/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(frog1) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog1/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog1/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog1/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog1/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(frog2) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog2/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog2/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog2/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog2/gradcam2.png?raw=true" width="180" height="180"> |

| Original image(frog3) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog3/original.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog3/heatmap.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog3/gradcam1.png?raw=true" width="180" height="180"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/frog3/gradcam2.png?raw=true" width="180" height="180"> |


**Observation**: From the sample results shown above, it seems like instead of focusing on the object itself, the model is mostly focusing on the contour/outline of the object (especially for the plane and the ship). Maybe this is due to the low resolution of the images or that the network is not deep enough. From the sample result of frog1, it seems like the model is learning to recognize the grass in the background to predict "frog", instead of looking at the frog itself. This may be due to low class number (only 10 classes), so the model doesn't need to know what a frog is, it just needs to learn enough to differentiate it from other classes.
