# Multi-site, Multi-domain Airway Tree Modeling


<!-- <div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/Lung_and_Airway.png"></div> -->
<div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/main_title.png"></div>

## Summary 
<p align = "justify"> 
Airway segmentation is a crucial step for the analysis of pulmonary diseases including asthma, bronchiectasis, and emphysema. The accurate segmentation based on X-Ray computed tomography (CT) enables the quantitative measurements of airway dimensions and wall thickness, which can reveal the abnormality of patients with chronic obstructive pulmonary disease (COPD). Besides, the extraction of patient-specific airway models from CT images is required for navigation in bronchoscopic-assisted surgery. Due to the fine-grained pulmonary airway structure, manual annotation is however time-consuming, error-prone, and highly relies on the expertise of clinicians. Bruijne et al. [1] held the ‘Extraction of airways from CT (EXACT'09)’ challenge in 2009 and achieved a great contribution to the field of airway segmentation. They focused on semi-automated and automated algorithms mainly based on multi-threshold, template matching, and region growing, aiming to relieve the burden of manual delineation and help clinicians explore the influence of pneumonia on airways. These traditional algorithms face difficulty in extracting small peripheral bronchi and suffer the risk of airway leakage. With the advance of deep learning methods, fully convolutional networks (FCNs) achieved state-of-the-art performance in the segmentation task of volumetric medical data. Most of the deep learning methods are data-driven while the EXACT’09 contains only 20 CT scans for training and 20 CT scans for testing, which is not sufficient for the artificial intelligence era. 
<br/>
<br/>
We collected 500 CT scans from multi-sites. The airway tree structures are carefully labeled by three radiologists with more than five years of professional experience.  
<br/>
<br/>
We encourage the participating teams to design robust algorithms, which can extract the airway tree structure with high topological completeness and accuracy for clinical use.
</p>

## Mission
The automatic airway segmentation algorithms are expected to be optimized to have the following properties:

* The completeness and the connectedness of the airway tree model. Only the largest component of the binary airway segmentation results are of clinical use and evaluated on the tree length detected rate (TD) and the branches detected rate (BD). 

* The accuracy of segmentation. We use the metric of the Dice similarity coefficient and Precision to measure the overlap-wise and pixel-wise segmentation accuracy, respectively.   



## <i class="fa-solid fa-calendar fa-2x"></i>  Timeline
<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 20 May 2022 </font>: Registration open.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 30 May 2022 </font> : Release of the training and validation data.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 15 July 2022 </font> : Deadline for validation submission.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 10 Aug 2022 </font> : Testing set opening.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 25 Aug 2022 </font> : Deadline for testing submission.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 18 Sep 2022 </font> : Top 10 teams’ results have been announced.


## <i class="fa-solid fa-person-chalkboard fa-2x"></i> Organizers
Prof. Guang-Zhong Yang (Institute of Medical Robotics, Shanghai Jiao Tong University)

Dr. Yun Gu (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Minghui Zhang (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Yangqian Wu (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Hanxiao Zhang (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Weihao Yu (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Hao Zheng (Institute of Medical Robotics, Shanghai Jiao Tong University)

Mr. Yulei Qin (Institute of Medical Robotics, Shanghai Jiao Tong University)

Prof. Jiayuan Sun (Department of Respiratory Endoscopy, Shanghai Chest hospital)




## <i class="fa-solid fa-database fa-2x"></i> Data
We collected 500 CT scans from multi-sites. The thoracic CT scans are collected from the public LIDC-IDRI dataset and the Shanghai Chest hospital. Each thoracic CT scan is first preprocessed by a strong deep learning model [2] to acquire the preliminary segmentation result and then delineated and double-checked by three radiologists with more than five years of professional experience to acquire the final refined airway tree structure. 
The annotation details can be seen [here](./annotation_detail.html).





<!-- ## Future
As we are dedicated to organizing the pulmonary airway segmentation challenge, more information, updates, and details will be included in this website. -->

### Reference

The airway segmentation works are provided: [Airway Segmentation Paper Reading Summary](https://drive.google.com/file/d/1s5fO4swUJGgHGCO9cDUoupGY1x9vCLMw/view?usp=sharing)

[1] Lo P, Van Ginneken B, Reinhardt J M, et al. Extraction of airways from CT (EXACT'09)[J]. IEEE Transactions on Medical Imaging, 2012, 31(11): 2093-2107.
<br/>
[2] Zheng H, Qin Y, Gu Y, et al. Alleviating Class-wise Gradient Imbalance for Pulmonary Airway Segmentation[J]. IEEE Transactions on Medical Imaging, 2021.



<head> 
    <script defer src="https://use.fontawesome.com/releases/v6.1.1/js/all.js"></script> 
    <script defer src="https://use.fontawesome.com/releases/v6.1.1/js/v4-shims.js"></script> 
</head> 
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.1.1/css/all.css">










