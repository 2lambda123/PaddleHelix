[English](README.md) | 简体中文

<p align="center">
<img src="./.github/飞桨-螺旋桨_logo.png" align="middle" height="75%" width="75%" />
</p>

------
[![Version](https://img.shields.io/github/release/PaddlePaddle/PaddleHelix.svg)](https://github.com/PaddlePaddle/PaddleHelix/releases)
![python version](https://img.shields.io/badge/python-3.6+-orange.svg)
![support os](https://img.shields.io/badge/os-linux%2C%20win%2C%20mac-yellow.svg)

螺旋桨（PaddleHelix）是一个基于机器学习的生物计算工具集，致力于加速如下领域的进展：
> * 疫苗设计
> * 新药发现
> * 精准医疗

## 特色

* **高性能**：提供了LinearRNA系列高性能算法助力 RNA 结构预测和分析。例如，LinearFold 和 LinearPartition 能够迅速准确定位能量较低 RNA 二级结构，性能相比传统方法提升数百甚至上千倍。
<p align="center">
<img src="./.github/LinearRNA.jpg" align="middle" />
</p>

* 由大规模**表示预训练**支撑的生物计算工具：随着自监督学习用于分子表示训练的进展，为样本量非常稀少的很多生物计算任务带来了全新的突破，这些任务包括分子性质预测，药物-靶点相互作用，蛋白质-蛋白质相互作用，RNA-RNA 相互作用，蛋白质折叠，RNA 折叠等等领域。螺旋桨广泛提供了业界最领先的表示学习方法和模型，使得开发者可以基于大规模模型快速切入需求的任务，站在巨人的肩膀上。
<p align="center">
<img src="./.github/paddlehelix_features.jpg" align="middle" />
</p>

* 丰富的样例和应用：螺旋桨提供了生物计算中常用的模块，如模型结构，数据集，和预训练模型。用户可以用非常简单的接口模块，快速组建自己的网络和系统。罗湘江还提供多种应用，例如化合物属性预测，药物靶点亲和力预测等等。
----

## 安装
详细的安装指引和环境配置请查阅[这里](./installation_guide_cn.md)。

----
## 文档

### 教学
* 我们提供了大量的[教学实例](./tutorials)以方便开发者快速了解和使用该框架
* PaddleHelix基于[飞桨（PaddlePaddle）](https://github.com/paddlepaddle/paddle)开源深度学习框架实现，该框架在性能表现上尤其出色。

### 使用示例
* [表示学习 - 化合物](./apps/pretrained_compound/README_cn.md)
* [表示学习 - 蛋白质](./apps/pretrained_protein/README_cn.md)
* [药物-分子作用预测](./apps/drug_target_interaction/README_cn.md)
* [分子生成](./apps/molecular_generation/README_cn.md)
* [药物联用](./apps/drug_drug_synergy/README_cn.md)
* [LinearRNA](./c/pahelix/toolkit/linear_rna/README_cn.md)

### API 文档
* 如果你对PaddleHelix的详细接口感兴趣，请查阅[API 文档](https://paddlehelix.readthedocs.io/en/dev/)。

### 开发者指南
* 如果你需要修改PaddleHelix的源代码，请查阅我们提供的[开发者指南](./developer_guide_cn.md)。

### 欢迎加入我们
我们正在招聘对人工智能驱动的药物设计感兴趣的机器学习研究人员/工程师或生物信息/计算化学相关研究人员。
我们的工作地点在中国深圳/上海。
请把简历寄到wangfan04@baidu.com 或者fangxiaomin01@baidu.com。
