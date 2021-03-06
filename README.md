# Group Behavior Recognition Using Attention- and Graph-Based Neural Networks

[[paper](https://ebooks.iospress.nl/volumearticle/55068)] [[video](https://underline.io/lecture/1953-group-behavior-recognition-using-attention--and-graph-based-neural-networks
)] [[data](https://sites.google.com/view/congreg8/home#h.p_FqKt0M9-taTN)]

If this code helps with your work, please cite:

```bibtex
@incollection{yang2020group,
  title={Group behavior recognition using attention-and graph-based neural networks},
  author={Yang, Fangkai and Yin, Wenjie and Inamura, Tetsunari and Bj{\"o}rkman, M{\aa}rten and Peters, Christopher},
  booktitle={ECAI 2020},
  pages={1626--1633},
  year={2020},
  publisher={IOS Press}
}
```

## Dataset

**CongreG8**: A mocap dataset for proxemics and social robotics (not public yet). Recorded in a motion capture lab with an approximate 5m × 5m × 3m active capture volume, which is equipped with a NaturalPoint Optitrack2 system with 16 Prime 41 cameras.

**Scenario**: A game scene called Who’s the Spy. Three group players and one observer. The observer approaches and joins the group. 

![network](https://github.com/YIN95/Group-Behavior-Recognition/blob/master/media/image1.png)

![network](https://github.com/YIN95/Group-Behavior-Recognition/blob/master/media/image2.gif)

**Details**: 
- 380 human approaches groups trials
- Full body motion capture data of all players (37 markers)
- Time period: 2-6 seconds;
- Frame rate: 120 fps;
- Behaviors: Accommodate and Ignore

## Methods

Based on Spatial-Temporal Graph Convolutional Networks (ST-GCN), but extended to multiple temporal scales (MST-GCN). Approach Group GCN (AG-GCN) for group behavior analysis: Multi-Spatial-Temporal GCN (MST-GCN) on the individual level and Group GCN on group level. 

![network](https://github.com/YIN95/Group-Behavior-Recognition/blob/master/media/image5.png)

## Demo

A use case in a virtual environment with live classification of accommodation and ignore.

![network](https://github.com/YIN95/Group-Behavior-Recognition/blob/master/media/image4.png)

## Acknowledgements

This code was built upon the [ST-GCN](https://github.com/yysijie/st-gcn) codebase and various recognition codebases. Many thanks to those authors for making their code available!

This research has received funding from the European Union‘s Horizon 2020 research and innovation programme under grant agreement n. 824160 (EnTimeMent).

