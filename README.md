# CardiacQuanNet
Synergistic Segmentation and Regression Learning for Cardiac MRI Left Ventricle Quantification Implementation

**Paper Abstract**

>Left ventricle (LV) scanning and morphological shape measurement are essential to improve the diagnosis of different cardiovascular diseases. In current clinical practice, LV quantification depend on the measurement of myocardial shape, which is usually performed using manual myocardial boundary delineation. However, this process is highly time-consuming and subjective to inter and intra-observer variability. In this paper, we propose a synergistic deep learning-based approach for full measurement of cardiac LV, including LV and myocardial cavities, regional wall thickness (RWT), LV dimensions, and cardiac phase cycle. We first segment cardiac LVs using an encoder-decoder network and then introduce a multitask framework for 11 LV indices regression and phase classification as a parallel task during the optimization. The proposed deep learning model is based on the Spatio-temporal convolution neural network (CNN) that extract spatial and temporal features from the identified region-of-interest (ROIs).
We demonstrate the efficacy of the proposed method on the MR sequence of 145 subjects, and in comparison to state-of-the-art quantification approaches. The proposed method achieved high accuracy prediction, with an average mean absolute error of 135 $mm^2$, 1.23 $mm$, 1.76 $mm$ for cavity regions, RWTs, dimensions, and an error rate of 9.0\% for phase classification. The experimental results highlight the robustness of the proposed method, despite varying degrees of cardiac morphology, image appearance, and low contrast in the cardiac MR sequences.

![alt text]()
