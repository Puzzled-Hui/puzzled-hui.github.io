# Annotation Details


## Pinciples
<p align = "justify"> 

We annotate the airway label based on the pre-trained model's segmentation. The annotation process contains the following principles:

* Consistency principle: We first make sure that each annotator uses the same principle to annotate. Referring to [1], we establish the rules considering the annotating details like branches annotation, lumen wall annotation, etc.

* Topology principle: To preserve the topological completeness of the airway labels, we manually annotate to repair some breakages and leakages in the pre-trained model's segmentation. We carefully relink the breakages and wipe out some small leakages based on the original CT features and anatomical prior knowledge.

</p>


## Examples
<p align = "justify">

We will give some specific examples during the annotation process, which contains the annotation for false negatives and false positives in the pre-trained model's segmentation.
</p>

<div align = center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/Annotation_details.png"></div>

<p align = "justify">

* For (a), we annotate to label the false negative in the pre-trained model's segmentation based on CT's feature and topological structure. The breakages in tiny bronchi are relinked to guarantee topological completeness.

* For (b), we annotate to remove the false positive in the pre-trained model's segmentation based on the feature of the original CT image. Those false positives are produced as they have the hole-like feature in the CT image. Therefore, they are removed by annotation to avoid overfitting in the training process.

</p>

### Reference
[1] Netter F H. Atlas of human anatomy, Professional Edition E-Book: including NetterReference. com Access with full downloadable image Bank[M]. Elsevier health sciences, 2014.

[back](./index.md)