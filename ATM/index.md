# Multi-site, Multi-domain Airway Tree Modeling


<!-- <div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/Lung_and_Airway.png"></div> -->
<div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/main_title.png"></div>

<!-- ## Summary 
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

* The accuracy of segmentation. We use the metric of the Dice similarity coefficient and Precision to measure the overlap-wise and pixel-wise segmentation accuracy, respectively.    -->
<p style= "text-align:justify">
<font color="firebrick" size=6><b> <i class="fa-solid fa-newspaper fa-2x"></i>  NEWS</b></font>
<br>
<font color="black"> 2022/04/19: Personal Challenge Website Open.</font>
<br>
<font color="black"> 2022/05/01: Official Website Open, Please refer to <i class="far fa-hand-point-right"></i> <a href="https://atm22.grand-challenge.org/"> Grand-Challenge Page</a> for participation.</font>
</p>

## <i class="fas fa-home fa-2x"></i> Home 
### <i class="fas fa-file-alt"></i> Background and Clinical Significance
<p style= "text-align:justify"> Airway segmentation is a crucial step for the analysis of pulmonary diseases including asthma, bronchiectasis, and emphysema. The accurate segmentation based on X-Ray computed tomography (CT) enables the quantitative measurements of airway dimensions and wall thickness, which can reveal the abnormality of patients with chronic obstructive pulmonary disease (COPD). Besides, the extraction of patient-specific airway models from CT images is required for navigation in bronchoscopic-assisted surgery. Due to the <b>fine-grained pulmonary airway structure</b>, manual annotation is however time-consuming, error-prone, and highly relies on the expertise of clinicians. </p>


### <i class="fas fa-edit"></i> Objective
<p style= "text-align:justify">
Bruijne et al. [1] held the ‘Extraction of airways from CT (EXACT'09)’ challenge in 2009 and achieved a great contribution to the field of airway segmentation. They focused on semi-automated and automated algorithms mainly based on multi-threshold, template matching, and region growing, aiming to relieve the burden of manual delineation and help clinicians explore the influence of pneumonia on airways. These traditional algorithms face difficulty in extracting small peripheral bronchi and suffer the risk of airway leakage. With the advance of deep learning methods, fully convolutional networks (FCNs) achieved state-of-the-art performance in the segmentation task of volumetric medical data. Most of the deep learning methods are data-driven while the EXACT’09 contains only 20 CT scans for training and 20 CT scans for testing, which is not sufficient for the artificial intelligence era. 

We collected 500 CT scans from multi-sites. The airway tree structures are carefully labeled by three radiologists with more than five years of professional experience. The intra-class imbalance among the trachea, main bronchi, lobar bronchi, and distal segmental bronchi affects the segmentation performance of peripheral bronchi. In conclusion, we encourage the participating teams to design robust algorithms, which can extract the airway tree structure with high <b> topological completeness </b> and <b> accuracy </b> for clinical use. Our challenge is open call (challenge opens for new submissions after conference deadline).
</p>

## <i class="fa-solid fa-calendar fa-2x"></i>  Timeline
<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 20 May 2022 </font>: Registration open.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 30 May 2022 </font> : Release of the training and validation data.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 15 July 2022 </font> : Deadline for validation submission.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 10 Aug 2022 </font> : Testing set opening.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 25 Aug 2022 </font> : Deadline for testing submission.

<i class="fa-solid fa-circle-chevron-right"></i> <font color=black> 18 Sep 2022 </font> : Top 10 teams’ results have been announced.


## <i class="fa-solid fa-person-chalkboard fa-2x"></i> Organizers
<p><font color=black> Prof. Guang-Zhong Yang </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Dr. Yun Gu </font> (Institute of Medical Robotics, Shanghai Jiao Tong University) <i class="fas fa-envelope"></i> <font color=black><b>Primary Contact</b></font>  </p> 
<p><font color=black> Mr. Minghui Zhang </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Mr. Yangqian Wu </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Mr. Hanxiao Zhang </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Mr. Weihao Yu </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Dr. Hao Zheng </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Dr. Yulei Qin </font> (Institute of Medical Robotics, Shanghai Jiao Tong University)</p>
<p><font color=black> Prof. Jiayuan Sun </font> (Department of Respiratory Endoscopy, Shanghai Chest hospital)</p>


## <i class="fa-solid fa-database fa-2x"></i> Dataset
<p style= "text-align:justify">
500 CT scans (300 for training, 50 for validation, 150 for testing) are collected from multi-sites. The thoracic CT scans are collected from the public LIDC-IDRI dataset [2] and the Shanghai Chest hospital. Each thoracic CT scan is first preprocessed by some strong deep learning models [3][4][5] and ensemble strategy to acquire the preliminary segmentation result and then carefullt delineated and double-checked by three radiologists with more than five years of professional experience to acquire the final refined airway tree structure.
<br> 
Please refer to <i class="far fa-hand-point-right"></i> <a href="./dataset_detail.html">Dataset Details</a> to be more familiar with the 
dataset structure, information, annotation details, etc,.
<br><i class="fas fa-book"></i> <b>Citation:</b> If using this dataset, you must cite the papers[3-6]. In addition, transfer of the dataset to others is not allowed! The challenge data and results will be free to use after the challenge results publication has been released. 
The organizers promise the blackout period will not be no longer than six months after the challenge is over.
</p>

## <i class="fas fa-cloud-upload fa-2x"></i> Submission Guideline
<p style= "text-align:justify">
<i class="fa-solid fa-1"></i> Please send the <a href="https://drive.google.com/file/d/1hIR7KKe_8zRO1Af1_6kuu5RGUqeqLlnQ/view?usp=sharing"> <font color="red"><b>signed document</b></font></a> to <a href="mailto:IMR-ATM22@outlook.com"> IMR-ATM22@outlook.com </a> for paticipation.
<br>  
<i class="fa-solid fa-2"></i> After investigatation, organizing committee will send the access of the data to the teams.
<br>
<i class="fa-solid fa-3"></i> All the registered teams should make a complete submission, containing:
<ul style="list-style-type:disc;">
<li>The docker container. The format of the docker file should follow: <i class="far fa-hand-point-right"></i> <a href="./docker_prepare.html"> Docker Submission Rule</a>. </li>
<li>A short paper, 2 pages at least, no more than 8 pages. Template same as MICCAI: <a href="https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines"> LNCS</a>.</li>
</ul>

<i class="fas fa-exclamation-triangle"></i> Only the <b>fully automatic</b> algorithms will be considered. Please send the docker container and 
the short paper to <a href="mailto:IMR-ATM22@outlook.com"> IMR-ATM22@outlook.com </a> via attachment or give the link to your submission, and then the organizer committee will download it.
</p>

## <i class="fas fa-balance-scale-left fa-2x"></i> Evaluation
<p style= "text-align:justify">
We aim to segment the accurate airway tree model. For one thing, only the largest component of the binary airway segmentation results are of clinical, to measure the completeness and the connectedness of the participating teams’ results, we use the tree length detected rate (TD) and the branches detected rate (BD). For another thing, we use the metric of the Dice similarity coefficient and Precision to measure the overlap-wise segmentation accuracy. Hence, we finally choose the following metrics:<br>
[1] Tree length detected rate (TD) and the branches detected rate (BD).
<br>
[2] Dice similarity coefficient (DSC) and Precision.
<br>
</p>
<div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/airway_parse.png"></div>
<p style= "text-align:justify">
Specifically, The TD is the fraction detected correctly relative to the total tree length in the reference label, and the
BD is the percentage of branches that are detected correctly with respect to the total number of branches present
in the reference label, as Fig.1 shows the parsing of the airway structure. The above metrics are commonly used in airway segmentations since 
the EXACT'09 Challenge [1].</p>


## <i class="fas fa-envelope fa-2x"></i> Contact Us
<p style= "text-align:justify"> If you have any questions about our challenge, please feel free to contact us.<br> Official Email: <a href="mailto:IMR-ATM22@outlook.com"> IMR-ATM22@outlook.com </a> | Primary Contact: <a href="mailto:geron762@sjtu.edu.cn "> geron762@sjtu.edu.cn </a>
</p>


### Reference
<p style= "text-align:justify">
Brief survey on airway segmentation: <a href="https://drive.google.com/file/d/1s5fO4swUJGgHGCO9cDUoupGY1x9vCLMw/view?usp=sharing"> IMR@SJTU_Airway_Segmentation_Survey.pdf </a>.<br>
[1] Lo P, Van Ginneken B, Reinhardt J M, et al. Extraction of airways from CT (EXACT'09)[J]. IEEE Transactions on Medical Imaging, 2012, 31(11): 2093-2107.
<br>
[2] Armato III S G, McLennan G, Bidaut L, et al. The lung image database consortium (LIDC) and image database resource initiative (IDRI): a completed reference database of lung nodules on CT scans[J]. Medical physics, 2011, 38(2): 915-931.
<br>
[3] Zheng H, Qin Y, Gu Y, et al. Alleviating Class-wise Gradient Imbalance for Pulmonary Airway Segmentation[J]. IEEE Transactions on Medical Imaging, 2021.
<br>
[4] Zhang M, Yu X, Zhang H, et al. FDA: Feature Decomposition and Aggregation for Robust Airway Segmentation[M]//Domain Adaptation and Representation Transfer, and Affordable Healthcare and AI for Resource Diverse Global Health. Springer, Cham, 2021: 25-34.
<br>
[5] Yu W, Zheng H, Zhang M, et al. BREAK: Bronchi Reconstruction by gEodesic transformation And sKeleton embedding[J]. arXiv preprint arXiv:2202.00002, 2022.
<br>
[6] Qin Y, Chen M, Zheng H, et al. Airwaynet: a voxel-connectivity aware approach for accurate airway segmentation using convolutional neural networks[C]//International Conference on Medical Image Computing and Computer-Assisted Intervention. Springer, Cham, 2019: 212-220.
</p>


<head> 
    <script defer src="https://use.fontawesome.com/releases/v6.1.1/js/all.js"></script> 
    <script defer src="https://use.fontawesome.com/releases/v6.1.1/js/v4-shims.js"></script> 
</head> 
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v6.1.1/css/all.css">










