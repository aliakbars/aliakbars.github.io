---
title: "Handling Missing Values in Healthcare Settings"
date: 2023-09-06
permalink: /posts/2023/09/missing-values
toc: true
redirect_from:
  - /rss23
tags:
  - missing-values
  - imputation
  - healthcare
---

[[Link]](https://virtual.oxfordabstracts.com/#/event/4019/submission/148) [[Slides]](https://1drv.ms/p/s!AhYtsNhF-mbvkgZxcfbgNPL-JGy_)

In statistical modeling, it is common to encounter missing values, particularly in healthcare situations where vital sign measurements may be sporadic. This can lead to difficulties in accurately evaluating a patient's health and making informed decisions about their treatment. One possible solution is to use imputation methods to fill in the missing values and enable counterfactual predictions in healthcare settings. To address this issue, we have conducted a study examining existing approaches to missing value imputation in healthcare settings, with a specific focus on time series data. We provide an overview of both classical (e.g. MICE, MissForest, Gaussian Processes), and deep learning-based (e.g. Recurrent Neural Networks, Generative Adversarial Networks, Autoencoders) imputation methods, assess their strengths and limitations within the context of time series data, and highlight potential areas for further investigation.

| Model             |   Year                                                                                                     | GP   | RNN   | CNN   | TF   | GAN   | ODE   | AE   | Indicator   | Datasets                                                    |
|:------------------|------------------------------------------------------------------------------------------------------------|:-----|:------|:------|:-----|:------|:------|:-----|:------------|:------------------------------------------------------------|
| MTGP              |  [2015](https://ojs.aaai.org/index.php/AAAI/article/view/9209)                                             | y    |       |       |      |       |       |      |             | TBI, MIMIC-II                                               |
| GASF, GADF, MTF   |  [2015](https://dl.acm.org/doi/10.5555/2832747.2832798)                                                    |      |       | y     |      |       |       |      |             | Gun Point, CBF, Swedish Leaf, ECG, 7 Misc                   |
| LSTM              |  [2016](http://proceedings.mlr.press/v56/Lipton16.html)                                                    |      | y     |       |      |       |       |      | y           | PICU at Children's Hospital LA                              |
| MTGP              |  [2017](http://proceedings.mlr.press/v70/futoma17a.html)                                                   | y    |       |       |      |       |       |      |             | Duke University Hospital                                    |
| M-RNN             |  [2017](https://ieeexplore.ieee.org/document/8485748)                                                      |      | y     |       |      |       |       |      |             | MIMIC-III, Deterioration, UNOS-Heart, UNOS-Lung, UK Biobank |
| BRITS             |  [2018](https://proceedings.neurips.cc/paper/2018/hash/734e6bfcd358e25ac1db0a4241b95651-Abstract.html)     |      | y     |       |      |       |       |      | y           | PhysioNet, Beijing Air Quality, Human Activity              |
| GRU-D             |  [2018](https://www.nature.com/articles/s41598-018-24271-9)                                                |      | y     |       |      |       |       |      | y           | PhysioNet, MIMIC-III, Gesture                               |
| GAIN              |  [2018](http://proceedings.mlr.press/v80/yoon18a.html)                                                     |      |       |       |      | y     |       |      |             | Breast Cancer, Spam, Letter, Credit, News                   |
| GP-VAE            |  [2019](https://arxiv.org/abs/1907.04155)                                                                  | y    |       | y     |      |       |       | y    |             | PhysioNet, Healing MNIST, SPRITES                           |
| T-CGAN            |  [2019](https://arxiv.org/abs/1811.08295)                                                                  |      |       |       |      | y     |       |      |             | Starlight Curves, Power Demand, ECG200                      |
| Imp-GAIN          |  [2019](https://dl.acm.org/doi/abs/10.1145/3292500.3330792)                                                |      |       |       |      | y     |       |      |             | Insomnia                                                    |
| Latent ODE        |  [2019](https://papers.nips.cc/paper_files/paper/2019/hash/42a6845a557bef704ad8ac9cb4461d43-Abstract.html) |      | y     |       |      |       | y     |      |             | PhysioNet, MuJoCo, Human Activity                           |
| VaDER             |  [2019](https://academic.oup.com/gigascience/article/8/11/giz134/5626377)                                  |      | y     |       |      |       |       | y    | y           | ADNI, PPMI                                                  |
| TKAE              |  [2019](https://dl.acm.org/doi/10.1016/j.patcog.2019.106973)                                               |      | y     |       |      |       |       | y    |             | PhysioNet, ECG, EHR                                         |
| ODE-GRU-D         |  [2020](https://ieeexplore.ieee.org/document/9180182)                                                      |      | y     |       |      |       | y     |      | y           | PhysioNet                                                   |
| RBM               |  [2020](https://www.sciencedirect.com/science/article/pii/S1532046420302045)                               |      |       |       |      |       |       | y    |             | Acute Abdomen Taiwan                                        |
| Multitask LSTM    |  [2020](https://dl.acm.org/doi/abs/10.1007/978-3-030-59137-3_5)                                            |      | y     |       |      |       |       |      |             | PhysioNet                                                   |
| HeartImp          |  [2020](https://epubs.siam.org/doi/10.1137/1.9781611976236.6)                                              |      |       |       |      |       |       | y    |             | Garmin, Fitbit                                              |
| GRU-DF            |  [2020](https://ieeexplore.ieee.org/document/9374359)                                                      |      | y     |       |      |       |       |      |             | CLIMB (Multiple Sclerosis)                                  |
| TAME              |  [2020](https://dl.acm.org/doi/10.1145/3394486.3403129)                                                    |      | y     |       |      |       |       | y    |             | MMIC-III, DACMI                                             |
| P-BiGAN           |  [2020](http://proceedings.mlr.press/v119/li20k.html)                                                      |      |       | y     |      | y     |       |      |             | MIMIC-III                                                   |
| Deep AE           |  [2021](https://ieeexplore.ieee.org/document/9238392)                                                      |      |       |       |      |       |       | y    |             | Ischemic Heart Disease Taiwan                               |
| Deep Recurrent AD |  [2021](https://www.sciencedirect.com/science/article/pii/S1053811921004201?via%3Dihub)                    |      | y     |       |      |       |       |      | y           | TADPOLE (ADNI)                                              |
| MTSIT             |  [2022](https://ieeexplore.ieee.org/document/9964035)                                                      |      |       |       | y    |       |       |      |             | PhysioNet, Beijing Air Quality                              |
| AJ-RNN            |  [2022](https://ieeexplore.ieee.org/document/9210118)                                                      |      | y     |       |      |       |       |      |             | PhysioNet, UCR Time Series                                  |

```bibtex
@article{septiandri2023missing,
  title   = {Handling Missing Values in Healthcare Settings},
  author  = {Septiandri, Ali Akbar and Jendoubi, Takoua and De la O, Alejandro Díaz},
  year    = 2023,
  month   = {September},
  url     = {https://aliakbars.id/posts/2023/09/missing-values}
}
```