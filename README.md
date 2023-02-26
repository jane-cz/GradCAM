# GradCAM
This repo contains 2 implementations of the GradCAM saliency map on the model provided in [this tutorial](https://captum.ai/tutorials/CIFAR_TorchVision_Interpret), on the CIFAR-10 dataset.
* The first implementation was adapted from [this tutorial](https://medium.com/@stepanulyanin/implementing-grad-cam-in-pytorch-ea0937c31e82).
* The second implementation directly used the [pytorch-grad-cam package](https://github.com/jacobgil/pytorch-grad-cam).

## Here are some sample results:

| Original image(plane) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/original.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/heatmap.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/gradcam1.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/plane/gradcam2.png?raw=true" width="256" height="256"> |

| Original image(ship1) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/original.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/heatmap.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/gradcam1.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship1/gradcam2.png?raw=true" width="256" height="256"> |

| Original image(ship2) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/original.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/heatmap.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/gradcam1.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/ship2/gradcam2.png?raw=true" width="256" height="256"> |

| Original image(cat) | Heatmap | GradCAM1 | GradCAM2 |
| ----------------------|------------------------------|-----------------------------|-------------------------------------|
| <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/original.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/heatmap.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/gradcam1.png?raw=true" width="256" height="256"> | <img src="https://github.com/jane-cz/GradCAM/blob/main/gradcam_img/cat/gradcam2.png?raw=true" width="256" height="256"> |


**Observation**: From the sample results, it seems like instead of focusing on the object itself, the model is mostly focusing on the contour/outline of the object (especially for the plane and the ship). Maybe this is due to the low resolution of the images or that the network is not deep enough.
