# Docker Preparation Guideline
<div align=center><img src="https://raw.githubusercontent.com/Puzzled-Hui/puzzled-hui.github.io/main/ATM/figures/titlepage.png"></div>

<!-- ## Under Construction ...  -->

## Test Phase Submission Guideline
<p style= "text-align:justify">
The participants should have some experience in the docker operations. The final docker tar file size must be less than 15 GB.
The docker should execute no more than 6 hours and occupy no more than 16 GB GPU Memory at best to generate the segmentation test results.
We will provide a GeForce RTX 3090 or a V100 for fair evaluation.
We are very grateful to the <a href="https://flare.grand-challenge.org/"> FLARE-challenge </a> that has provided the materials for the docker 
tutorial, we will follow these formats.
The docker should be saved with (please do not use capital letters in the teamname): 
<br> 
<font size="5"><code>  docker save teamname:latest -o teamname.tar.gz  </code></font>
<br> 
The submitted docker should be named as `teamname.tar.gz` (teamname should be lowercase letters). The samples in the test set are evaluated one-by-one by runing the docker with:
<br> 
<code>docker image load < teamname.tar.gz</code>
<br> 
<code>docker container run --gpus "device=1" --name teamname --rm -v $PWD/inputs/:/workspace/inputs/ -v $PWD/teamname_outputs/:/workspace/outputs/ teamname:latest /bin/bash -c "sh predict.sh"</code>
<br> 
<br> 
<i class="fas fa-exclamation-triangle"></i> NOTE:
We will mount the $PWD/inputs/ [a folder contains testing cases, file structure is same as the training and validation] to /workspace/inputs/ in your docker container, and and mount $PWD/teamname_outputs/ [an empty folder used to save individual prediction results] to /workspace/outputs/ in your docker container.
<br>
Your docker container should do the following things:
<br>
1. Load each CT file (.nii.gz) in /workspace/inputs/
<br>
2. Apply the automatic segmentation algorithm.
<br>
3. Save the binary result to /workspace/outputs/. Note that the filename of binary result should be the same as the input CT file.
<br>
We will provide a tiny testset for you to prepare the whole pipeline.

<br>
There are some useful public links that we recommend for you in case you are not familiar with the docker.
<br>
<a href="https://github.com/YaoZhang93/FLARE2021-Baseline"> Docker Example 1  </a>

<a href="https://github.com/PerceptionComputingLab/PARSE2022/blob/main/docker_rules/docker-submission-rules.md"> Docker Example 2 </a>
</p>

## Validation Phase Submission Guideline
<p style= "text-align:justify">
In regard to the validation phase, we open a validation phase in the grand-challenge, in this phase, you should:
<br>
Step 1. Submit the short paper in the supplementary file of Validation Phase or Email a short paper to IMR-ATM22@outlook.com.
<br>
Step 2. Submit the compressed binary segmentation result (e.g., teamnameVal1.zip) on the Validation Phase.  Folder structure:
<br>
teamnameVal1/<br>
|————ATM_301_0000.nii.gz<br>
|————ATM_302_0000.nii.gz<br>
...<br>
|————ATM_350_0000.nii.gz<br>
TIPS: The number index is not exactly from 301-350, but the total count is 50 as scheduled.<br>
Three time submissions on the validation set are allowed, each submission should be associated with independent short papers.
</p>











