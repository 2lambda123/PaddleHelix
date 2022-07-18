# HelixFold 

<p align="center">
<img src="../../../.github/helixfold_pipeline.png" align="middle" height="90%" width="90%" />
</p>

------

Reproduction of [AlphaFold 2](https://doi.org/10.1038/s41586-021-03819-2) with [PaddlePaddle](https://github.com/paddlepaddle/paddle).

[HelixFold](https://arxiv.org/abs/2207.05477) currently provides a PaddlePaddle implementation of the AlphaFold training and inference pipeline in GPU and DCU. We try to reproduce all the training details as stated in the AF2 paper. As for the inference pipeline, we reproduce exactly the same results as the original open source inference codes (v2.0.1) including recycle and ensembling.

The installation prerequisites are different for the training and inference pipeline in GPU and DCU. The following links provide detailed instructions on running HelixFold.

* [Training Pipeline in GPU](README_train.md)
* [Training Pipeline in DCU](README_DCU.md)
* [Inference Pipeline in GPU](README_inference.md)

## Highlights

### Branch Parallelism and Hybrid Parallelism

HelixFold proposes Branch Parallelism (BP) to split the calculation branch across multiple devices in order to accelerate computation during initial training phase. The training cost is further reduced by combining BP with Dynamic Axial Parallelism (DAP) and Data Parallelism (DP).

<p align="center">
<img src="../../../.github/BP_DAP_DP.png" align="middle" height="90%" width="90%" />
</p>

## Copyright

HelixFold code is licensed under the Apache 2.0 License, which is same as AlphaFold. However, we use the AlphaFold parameters pretrained by DeepMind, which are made available for non-commercial use only under the terms of the CC BY-NC 4.0 license.

## Reference

[1] Jumper J, Evans R, Pritzel A, et al. Highly accurate protein structure prediction with AlphaFold[J]. Nature, 2021, 596(7873): 583-589.

## Citation

If you find our work is helpful to your research, please cite:

```
@article{wang2022helixfold,
  title={HelixFold: An Efficient Implementation of AlphaFold2 using PaddlePaddle},
  author={Wang, Guoxia and Fang, Xiaomin and Wu, Zhihua and Liu, Yiqun and Xue, Yang and Xiang, Yingfei and Yu, Dianhai and Wang, Fan and Ma, Yanjun},
  journal={arXiv preprint arXiv:2207.05477},
  year={2022}
}
```
