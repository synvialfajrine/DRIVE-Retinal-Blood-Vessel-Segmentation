# DRIVE Retinal Blood Vessel Segmentation 

Retinal fundus imaging is useful for the diagnosis, screening, and screening of cardiovascular
and ophthalmic diseases, including age-related macular degeneration (AMD), diabetic
retinopathy (DR), glaucoma, hypertension, atherosclerosis, and choroidal neovascularization,
where AMD and DR are believed to be the two main causes of blindness [1].

Vessel segmentation is one of approaches for analyzing retinal fundus images. The segmented
vascular tree can be used to extract the morphological attributes of blood vessels, such as
length, width, branching and angles [1].

Manual segmentation of the vascular tree in retinal images is a tedious task that requires
experience and skill. Additionally, it has time-consuming process. In this assignment, retinal
blood vessel segmentation is done using morphological operators.

## Dataset
Dataset used in this assigment is taken from DRIVE dataset, that can be retrieved from this [link](https://drive.grand-challenge.org/DRIVE/). It is an openly available dataset consisting of 40 images of size 565 × 584 pixels.

## Steps
Segmentation steps applied to DRIVE dataset:
1. Extracting green channel from RGB image
2. Applying CLAHE to green channel image
3. Estimating background using morphology operation
4. Substracting image to its estimated background
5. Applying CLAHE and median filter to the substracted image to get the vessel segmentation.

## Performance Average
Accuracy = 92.74210510364892
Specificity = 94.30718771798416
Sensitivity = 76.64419658324289
F1 Score = 65.02933357773861

## Conclusion
The approach applied to segment retinal vessel has high accuracy and specificity but still needs
improvement to get better result. The segmented images have noises and the vessel pixels can
not be detected thoroughly. There are some vessel pixels that loses in the segmentation
process.

## References
1. Q. Li, B. Feng, L. Xie, P. Liang, H. Zhang and T. Wang, "A Cross-Modality Learning Approach
for Vessel Segmentation in Retinal Images," in IEEE Transactions on Medical Imaging, vol. 35,
no. 1, pp. 109-118, Jan. 2016, doi: 10.1109/TMI.2015.2457891.
2. Özkaya, Umut & Öztürk, Şaban & Akdemir, Bayram & Seyfi, Levent, "An Efficient Retinal
Blood Vessel Segmentation using Morphological Operations", 2018, pp. 1-7,
10.1109/ISMSIT.2018.8567239.
3. Digital Retinal Images for Vessel Extraction (DRIVE). Available at (https://drive.grand-challenge.org/DRIVE/)[[https://drive.grandchallenge.org/DRIVE/](https://drive.grand-challenge.org/DRIVE/)https://drive.grand-challenge.org/DRIVE/]
