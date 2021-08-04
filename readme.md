## TransCenter: Transformers with Dense Queries for Multiple-Object Tracking <br />
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

**TransCenter: Transformers with Dense Queries for Multiple-Object Tracking** <br />
[Yihong Xu](https://team.inria.fr/perception/team-members/yihong-xu/), [Yutong Ban](https://team.inria.fr/perception/team-members/yutong-ban/), [Guillaume Delorme](https://team.inria.fr/robotlearn/team-members/guillaume-delorme/), [Chuang Gan](https://people.csail.mit.edu/ganchuang/), [Daniela Rus](http://danielarus.csail.mit.edu/), [Xavier Alameda-Pineda](http://xavirema.eu/) <br />
**[[Paper](https://arxiv.org/abs/2103.15145)]** <br />

<div align="center">
  <img src="https://github.com/yihongXU/TransCenter/raw/main/pipeline.png" width="1200px" />
</div>


## Acknowledgement <a name="Acknowledgement">
The code for TransCenter is modified and network pre-trained weights are obtained from the following repositories: <br />

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
**MOT Metrics in Python**: [**py-motmetrics**](https://github.com/cheind/py-motmetrics)<br />
**Soft-NMS**: [**Soft-NMS**](https://github.com/DocF/Soft-NMS)<br />
**DETR**: [**DETR**](https://github.com/facebookresearch/detr)<br />
