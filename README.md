# 3D-thresholding
An ImageJ-Script that runs the local thresholding algorithms included in ImageJ on three orthogonal reconstructions of the source data.

This is the standalone version (one-method, one-radius 3D thresholding) of the method described in the paper "VOLT: a novel open-source pipeline for automatic segmentation of endolymphatic space in inner ear MRI" (https://pubmed.ncbi.nlm.nih.gov/32666134/), simply as a imageJ-Macro. Depending on your data quality, you will need some preprocessing, e.g., noise correction or contrast enhancement. 

If you want to automatize the whole process, just remove the dialog window, and define one radius  for all datasets. Again, you will have to finetune this to your specific data. We ended up using two algorithms and four radii, and averaging the results (e.g., by using a z-projection of a 4D-hyperstack in ImageJ), but it might be that other approaches give better results in your case. 

For the DL-segmentation, we used IE VNET (https://github.com/pydsgz/IEVNet).
