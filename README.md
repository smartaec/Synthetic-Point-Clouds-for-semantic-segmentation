# Synthetic-Point-Clouds-for-semantic-segmentation
The results for the paper "Impact of color and mixing proportion of synthetic point clouds on semantic segmentation"

## Introduction
In the paper, we propose a method for generating synthetic point clouds (SPC) based on BIM models, and explore the 
impact of the mixing proportions (synthetic & real point clouds) on the training performance of semantic segmentation 
models. The impact of the mixing proportions between synthetic and real point clouds on the training of PointNet, 
PointNet++, and DGCNN models has been presented in the paper. At the same time, we are actively exploring the potential 
of SPC on more advanced semantic segmentation models or network architectures.  
The latest results will be continuously updated in this repository. 

## Results
### Statement  
#### Experiments Info
**SPC proportion**: the proportion of SPC to the total number of point clouds in the training 
set (proportion of scene quantity).  
**mixing training**: experiments of mixed training of synthetic and real point clouds with certain SPC proportions.  
**benchmark**: remove SPC from mixing training as benchmark experiments

#### Evaluation Metrics  
**mIoU**: mean Intersection over Union.  
**OA**: Overall Accuracy.  
**OA<sub>7</sub>**: overall accuracy not considering "clutter" class.

#### legend
<div style="text-align: center;">
  <img src="Results/Legend.jpg" alt="DGCNN_mIoU" style="max-width: 68%; height: auto;">
</div>

### PointNet (CVPR 2017) [[paper](https://web.stanford.edu/~rqi/pointnet/)]
<div style="text-align: center;">
  <img src="Results/PointNet/mIoU.jpg" alt="PointNet_mIoU" style="max-width: 32%; height: auto;">
  <img src="Results/PointNet/OA.jpg" alt="PointNet_OA" style="max-width: 32%; height: auto;">
  <img src="Results/PointNet/OA7.jpg" alt="PointNet_OA7" style="max-width: 32%; height: auto;">
</div>

### PointNet++ (NIPS 2017) [[paper](https://web.stanford.edu/~rqi/pointnet2/)]
<div style="text-align: center;">
  <img src="Results/PointNet2/mIoU.jpg" alt="PointNet++_mIoU" style="max-width: 32%; height: auto;">
  <img src="Results/PointNet2/OA.jpg" alt="PointNet++_OA" style="max-width: 32%; height: auto;">
  <img src="Results/PointNet2/OA7.jpg" alt="PointNet++_OA7" style="max-width: 32%; height: auto;">
</div>

### DGCNN (ACM TOG 2019) [[arXiv](https://arxiv.org/pdf/1801.07829)]
<div style="text-align: center;">
  <img src="Results/DGCNN/mIoU.jpg" alt="DGCNN_mIoU" style="max-width: 32%; height: auto;">
  <img src="Results/DGCNN/OA.jpg" alt="DGCNN_OA" style="max-width: 32%; height: auto;">
  <img src="Results/DGCNN/OA7.jpg" alt="DGCNN_OA7" style="max-width: 32%; height: auto;">
</div>

### Point Transformer (ICCV 2021) [[arXiv](https://arxiv.org/abs/2012.09164)]
<div style="text-align: center;">
  <img src="Results/PTv1/mIoU.jpg" alt="PTv1_mIoU" style="max-width: 32%; height: auto;">
  <img src="Results/PTv1/OA.jpg" alt="PTv1_OA" style="max-width: 32%; height: auto;">
  <img src="Results/PTv1/OA7.jpg" alt="PTv1_OA7" style="max-width: 32%; height: auto;">
</div>
