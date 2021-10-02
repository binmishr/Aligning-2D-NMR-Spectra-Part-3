# Aligning-2D-NMR-Spectra-Part-3

The details of the codeset and plots are included in the attached Adobe Acrobat reader (.pdf) file in this repository. 
You need to download the same to view the contents. There are referrals to other contents in BLUE colour also to follow.

A Brief Introduction
======================

Let’s get to work. The function to carry out alignment is hats_alignSpectra2D. The arguments maxF1 and maxF2 define the space that will be considered as the two spectra are shifted relative to each other. The space potentially covered is -maxF1 to maxF1 and similarly for the F2 dimension. dist_method, thres and minimize refer to the objective function. In this example we will consider two spectra succcessfully aligned when we get below the threshold. When one shifts one spectrum relative to the other, part of the shifted spectrum gets cutoff and part of it is empty space. fill = "noise" instructs the function to fill the empty space with an estimate of the noise from the original spectrum. We’ll set plot = FALSE here because the output is extensive.
