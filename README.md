# pl-sem-seg
Repository for implementation and training of semantic segmentation models using PyTorch Lightning

## Dataset Used
The [KITTI semantic segmentation dataset](http://www.cvlibs.net/datasets/kitti/eval_semseg.php?benchmark=semantics2015) is used in this. So, it needs to be downloaded from above link. It is used for it's small size (200 semantically annotated images and 200 test images). Data preprocessing and loading is as per this dataset. This dataset claims to be same in format to [Cityscapes](https://www.cityscapes-dataset.com/) (a much larger dataset of road scenes), so same code can be used with some modifications (not done in this yet, due to memory limitations).

## Models Implemented
- FCN ResNet50/101 (available through [torchvision.models.segmentation](https://pytorch.org/docs/stable/torchvision/models.html#semantic-segmentation))
- DeepLabv3 ResNet50/101 (available through [torchvision.models.segmentation](https://pytorch.org/docs/stable/torchvision/models.html#semantic-segmentation))
- [U-net](https://lmb.informatik.uni-freiburg.de/people/ronneber/u-net/)