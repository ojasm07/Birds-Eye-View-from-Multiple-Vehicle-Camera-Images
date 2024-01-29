# Birds-Eye-View-from-Multiple-Vehicle-Camera-Images

This repository contains the implementation of our methodology to obtain a bird’s-eye view (BEV) image from multiple vehicle-mounted camera images. Implemented a U-Net architecture featuring homography-enabled Transformers with a multi-input encoder-decoder framework. The model utilizes SegFormer for obtaining semantically segmented real images. Implemented Inverse Perspective Mapping (IPM) to improve spatial consistency.

**Dataset**: CARLA simulator dataset (comprising images from left, right, front, rear-view cameras, and an aerial top-down view from a drone’s perspective).

**Training Environment**: AWS g5.4xLarge instance with NVIDIA A100 Tensor Core GPUs, 24GiB GPU Memory, 16 vCPUs, 600GiB CPU Memory.

## Results
Our methodology achieved a Mean Intersection-over-Union (MIoU) of 55.31% on the validation set. Class IoU scores further validate the effectiveness of our model, particularly in predicting large-area semantic classes.