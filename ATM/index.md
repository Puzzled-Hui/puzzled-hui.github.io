# Multi Site Airway Tree Modeling (ATM'22)


<div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/Lung_and_Airway.png"></div>


## Summary 
<p align = "justify"> 
Airway segmentation is a crucial step for the analysis of pulmonary diseases including asthma, bronchiectasis, and emphysema. The accurate segmentation based on X-Ray computed tomography (CT) enables the quantitative measurements of airway dimensions and wall thickness, which can reveal the abnormality of patients with chronic obstructive pulmonary disease (COPD). Besides, the extraction of patient-specific airway models from CT images is required for navigation in bronchoscopic-assisted surgery. Due to the fine-grained pulmonary airway structure, manual annotation is however time-consuming, error-prone, and highly relies on the expertise of clinicians.  
<br/>
<br/>
We collected 500 CT scans from multi-sites and multi-domains. The airway tree structures are carefully labeled by three radiologists with more than five years of professional experience.  
<br/>
<br/>
We encourage the participating teams to design robust algorithms, which can extract the airway tree structure with high topological completeness and accuracy for clinical use.
</p>

## Mission of The Challenge
The automatic airway segmentation algorithms are expected to be optimized to have the following properties:

* The completeness and the connectedness of the airway tree model. Only the largest component of the binary airway segmentation results are of clinical use and evaluated on the tree length detected rate (TD) and the branches detected rate (BD). 

* The accuracy of segmentation. We use the metric of the Dice similarity coefficient and Precision to measure the overlap-wise and pixel-wise segmentation accuracy, respectively.   

















