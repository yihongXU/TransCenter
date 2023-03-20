## TransCenter: Transformers with Dense Representations for Multiple-Object Tracking <br />
## The work is accepted for TPAMI 2022.
## An update towards a more efficient and powerful TransCenter, TransCenter-Lite! ##

## The code for TransCenterV2 and TransCenter-Lite is now available, you can find the code and pretrained models at https://gitlab.inria.fr/robotlearn/TransCenter_official.

**TransCenter: Transformers with Dense Representations for Multiple-Object Tracking** <br />
[Yihong Xu](https://team.inria.fr/robotlearn/team-members/yihong-xu/), [Yutong Ban](https://people.csail.mit.edu/yban/index.html), [Guillaume Delorme](https://team.inria.fr/robotlearn/team-members/guillaume-delorme/), [Chuang Gan](https://people.csail.mit.edu/ganchuang/), [Daniela Rus](http://danielarus.csail.mit.edu/), [Xavier Alameda-Pineda](http://xavirema.eu/) <br />
**[[Paper](https://arxiv.org/abs/2103.15145)]** **[[Project](https://team.inria.fr/robotlearn/transcenter-transformers-with-dense-queriesfor-multiple-object-tracking/)]**<br />

<div align="center">
  <img src="https://github.com/yihongXU/TransCenter/raw/main/eTransCenter_pipeline.png" width="1200px" />
</div>

<br /><br />
**MOT20 example: <br />
![](https://github.com/yihongXU/TransCenter/blob/main/transcenter_mot20_example.gif)


## Bibtex
**If you find this code useful, please star the project and consider citing:** <br />
```
@misc{xu2021transcenter,
      title={TransCenter: Transformers with Dense Representations for Multiple-Object Tracking}, 
      author={Yihong Xu and Yutong Ban and Guillaume Delorme and Chuang Gan and Daniela Rus and Xavier Alameda-Pineda},
      year={2021},
      eprint={2103.15145},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```


## MOTChallenge Results

***For TransCenter V2***:

MOT17 public detections:
     
| Pretrained| MOTA     | MOTP     | IDF1 |  FP    | FN    | IDS |
|-----------|----------|----------|--------|-------|------|----------------|
|   CoCo  |  71.9%   |  80.5%   | 64.1% | 27,356  | 126,860  |     4,118     |
|   CH    |  75.9%   |  81.2%   | 65.9%  | 30,190 | 100,999 |     4,626    |

MOT20 public detections:
   
| Pretrained| MOTA     | MOTP     | IDF1 |  FP    | FN    | IDS |
|-----------|----------|----------|--------|-------|------|----------------|
|   CoCo    |  67.7%   |  79.8%   | 58.9%  | 54,967   | 108,376  |     3,707     |
|   CH      |  72.8%   |  81.0%   | 57.6%  | 28,026  | 110,312  |     2,621     |


MOT17 private detections:
   
| Pretrained| MOTA     | MOTP     | IDF1 |  FP    | FN    | IDS |
|-----------|----------|----------|--------|-------|------|----------------|
|   CoCo  |  72.7%   |  80.3%   | 64.0% | 33,807   | 115,542  |    4,719     |
|   CH    |  76.5%   |  81.1%   | 65.5% | 40,101 | 88,827 |     5,394    |

MOT20 private detections:

| Pretrained| MOTA     | MOTP     | IDF1 |  FP    | FN    | IDS |
|-----------|----------|----------|--------|-------|------|----------------|
|   CoCo   |  67.7%   |  79.8%   | 58.7% | 56,435  | 107,163 |     3,759     |
|   CH   |  72.9%   |  81.0%   | 57.7%  | 28,596  | 108,982  |     2,625     |


**Note:** 
- The results can be slightly different depending on the running environment.
- We might keep updating the results in the near future.

## Acknowledgement

The code for TransCenterV2, TransCenter-Lite is modified and network pre-trained weights are obtained from the following repositories:

1) The PVTv2 backbone pretrained models from PVTv2.
2) The data format conversion code is modified from CenterTrack.

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

@article{zhang2021bytetrack,
  title={ByteTrack: Multi-Object Tracking by Associating Every Detection Box},
  author={Zhang, Yifu and Sun, Peize and Jiang, Yi and Yu, Dongdong and Yuan, Zehuan and Luo, Ping and Liu, Wenyu and Wang, Xinggang},
  journal={arXiv preprint arXiv:2110.06864},
  year={2021}
}

@article{wang2021pvtv2,
  title={Pvtv2: Improved baselines with pyramid vision transformer},
  author={Wang, Wenhai and Xie, Enze and Li, Xiang and Fan, Deng-Ping and Song, Kaitao and Liang, Ding and Lu, Tong and Luo, Ping and Shao, Ling},
  journal={Computational Visual Media},
  volume={8},
  number={3},
  pages={1--10},
  year={2022},
  publisher={Springer}
}
```
Several modules are from:

**MOT Metrics in Python**: [**py-motmetrics**](https://github.com/cheind/py-motmetrics)

**Soft-NMS**: [**Soft-NMS**](https://github.com/DocF/Soft-NMS)

**DETR**: [**DETR**](https://github.com/facebookresearch/detr)

**DCNv2**: [**DCNv2**](https://github.com/CharlesShang/DCNv2)

**PVTv2**: [**PVTv2**](https://github.com/whai362/PVT)

**ByteTrack**: [**ByteTrack**](https://github.com/ifzhang/ByteTrack)

