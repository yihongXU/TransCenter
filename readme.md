## TransCenter: Transformers with Dense Queries for Multiple-Object Tracking <br />
## TransCenter's code is now available, you can find the code and pretrained models at https://gitlab.inria.fr/yixu/TransCenter_official.
**TransCenter: Transformers with Dense Queries for Multiple-Object Tracking** <br />
[Yihong Xu](https://team.inria.fr/robotlearn/team-members/yihong-xu/), [Yutong Ban](https://team.inria.fr/perception/team-members/yutong-ban/), [Guillaume Delorme](https://team.inria.fr/robotlearn/team-members/guillaume-delorme/), [Chuang Gan](https://people.csail.mit.edu/ganchuang/), [Daniela Rus](http://danielarus.csail.mit.edu/), [Xavier Alameda-Pineda](http://xavirema.eu/) <br />
**[[Paper](https://arxiv.org/abs/2103.15145)]** **[[Project](https://team.inria.fr/robotlearn/transcenter-transformers-with-dense-queriesfor-multiple-object-tracking/)]**<br />

<div align="center">
  <img src="https://github.com/yihongXU/TransCenter/raw/main/pipelineV2.png" width="1200px" />
</div>

## Bibtex
If you find this code useful, please star the project and consider citing:

```
@misc{xu2021transcenter,
      title={TransCenter: Transformers with Dense Queries for Multiple-Object Tracking}, 
      author={Yihong Xu and Yutong Ban and Guillaume Delorme and Chuang Gan and Daniela Rus and Xavier Alameda-Pineda},
      year={2021},
      eprint={2103.15145},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```


## Acknowledgement

The code for TransCenter is modified and network pre-trained weights are obtained from the following repositories:

1) The Person Reid Network  (./tracking/transcenter/model_zoo/ResNet_iter_25245.pth) is from Tracktor.
2) The lightflownet pretrained model (./tracking/transcenter/util/LiteFlownet/network-kitti.pytorch) is from pytorch-liteflownet and LiteFlowNet.
3) The deformable transformer pretrained model (./model_zoo/r50_deformable_detr-checkpoint.pth) is from Deformable-DETR.
4) The data format conversion code is modified from CenterTrack.

[**CenterTrack**](https://github.com/xingyizhou/CenterTrack), [**Deformable-DETR**](https://github.com/fundamentalvision/Deformable-DETR), [**Tracktor**](https://github.com/phil-bergmann/tracking_wo_bnw).
```
@article{zhou2020tracking,
  title={Tracking Objects as Points},
  author={Zhou, Xingyi and Koltun, Vladlen and Kr{\"a}henb{\"u}hl, Philipp},
  journal={ECCV},
  year={2020}
}

@InProceedings{tracktor_2019_ICCV,
author = {Bergmann, Philipp and Meinhardt, Tim and Leal{-}Taix{\'{e}}, Laura},
title = {Tracking Without Bells and Whistles},
booktitle = {The IEEE International Conference on Computer Vision (ICCV)},
month = {October},
year = {2019}}

@article{zhu2020deformable,
  title={Deformable DETR: Deformable Transformers for End-to-End Object Detection},
  author={Zhu, Xizhou and Su, Weijie and Lu, Lewei and Li, Bin and Wang, Xiaogang and Dai, Jifeng},
  journal={arXiv preprint arXiv:2010.04159},
  year={2020}
}
```
Several modules are from:

**MOT Metrics in Python**: [**py-motmetrics**](https://github.com/cheind/py-motmetrics)

**Soft-NMS**: [**Soft-NMS**](https://github.com/DocF/Soft-NMS)

**DETR**: [**DETR**](https://github.com/facebookresearch/detr)

**DCNv2**: [**DCNv2**](https://github.com/CharlesShang/DCNv2)

**correlation_package**: [**correlation_package**](https://github.com/NVIDIA/flownet2-pytorch/tree/master/networks/correlation_package)

**pytorch-liteflownet**: [**pytorch-liteflownet**](https://github.com/sniklaus/pytorch-liteflownet)

**LiteFlowNet**: [**LiteFlowNet**](https://github.com/twhui/LiteFlowNet)
```
@InProceedings{hui18liteflownet,
    author = {Tak-Wai Hui and Xiaoou Tang and Chen Change Loy},
    title = {LiteFlowNet: A Lightweight Convolutional Neural Network for Optical Flow Estimation},
    booktitle  = {Proceedings of IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
    year = {2018},
    pages = {8981--8989},
    }
```
