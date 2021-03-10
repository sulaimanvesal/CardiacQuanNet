# Spatio-temporal Multi-task Learning for Cardiac MRI Left Ventricle Quantification

TensorFlow/Keras implementation of our method for [Spatio-temporal Multi-task Learning for Cardiac MRI Left Ventricle Quantification](https://ieeexplore.ieee.org/abstract/document/9302580). Based on this implementation, our result achieved state-of-the-art performance for [LVquan 2018 Benchmark Dataset](https://lvquan18.github.io/). This paper has been published at [IEEE Journal of Biomedical and Health Informatics](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6221020)

### Contact: Sulaiman Vesal (sulaiman dot vesal at fau dot com)

---
**Paper Abstract**

>Left ventricle (LV) scanning and morphological shape measurement are essential to improve the diagnosis of different cardiovascular diseases. In current clinical practice, LV quantification depend on the measurement of myocardial shape, which is usually performed using manual myocardial boundary delineation. However, this process is highly time-consuming and subjective to inter and intra-observer variability. In this paper, we propose a synergistic deep learning-based approach for full measurement of cardiac LV, including LV and myocardial cavities, regional wall thickness (RWT), LV dimensions, and cardiac phase cycle. We first segment cardiac LVs using an encoder-decoder network and then introduce a multitask framework for 11 LV indices regression and phase classification as a parallel task during the optimization. The proposed deep learning model is based on the Spatio-temporal convolution neural network (CNN) that extract spatial and temporal features from the identified region-of-interest (ROIs).
We demonstrate the efficacy of the proposed method on the MR sequence of 145 subjects, and in comparison to state-of-the-art quantification approaches. The proposed method achieved high accuracy prediction, with an average mean absolute error of 135 $mm^2$, 1.23 $mm$, 1.76 $mm$ for cavity regions, RWTs, dimensions, and an error rate of 9.0\% for phase classification. The experimental results highlight the robustness of the proposed method, despite varying degrees of cardiac morphology, image appearance, and low contrast in the cardiac MR sequences.

![framework](Lvgit.png)


## Installation

* Install TensorFlow/Keras from http://tensorflow.org with Python 3.6 and CUDA 10.0

* NEW Add the LS-GAN objective to improve the performance

* Usage: add --gan LS option during training (see below for more details)
PyTorch 0.4 with Python 3 and CUDA 8.0

* Usage: replace the training and evaluation codes with the ones in the pytorch_0.4 folder
Update: tensorboard is provided by adding --tensorboard in the command
Note: the single-level model works as expected, while the multi-level model requires smaller weights, e.g., --lambda-adv-target1 0.00005 --lambda-adv-target2 0.0005. We will investigate this issue soon.

* Clone this repo
```
git clone https://github.com/sulaimanvesal/CardiacQuanNet/
cd CardiacQuanNet
```
## Dataset
* Download the LV-Quan 2018 Dataset put it in the data/GTA5 folder 
* https://lvquan18.github.io/

## Testing
---
## Citations
Please consider citing the following papers in your publications if they help your research.
```
@ARTICLE{9302580,
  author={S. {Vesal} and M. {Gu} and A. {Maier} and N. {Ravikumar}},
  journal={IEEE Journal of Biomedical and Health Informatics}, 
  title={Spatio-temporal Multi-task Learning for Cardiac MRI Left Ventricle Quantification}, 
  year={2020},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/JBHI.2020.3046449}}
```
