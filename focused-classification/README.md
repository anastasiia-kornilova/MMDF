### In-focus/out-of-focus classification

Despite auto-focusing systems in modern microscopes, obtained images are still should be filtered out to remove blurred images with artefacts, to find planes of one specimen with different focused areas. In comparison to classical focus measure operators, Deep Learning techniques allow not to lose small focused parts of the image and ignore artifacts in optical system (dust, drops, condensate).

In our comparison we consider the most significant operators from microscopy focus measure operators reviews (Laplacian, Tenengrad, Vollath), original pre-trained model from the paper "Assessing microscope image focus quality with deep learning" and our upgraded model. We also took into comparison a popular pre-trained model for non-microscopic images from the paper  "Blurred image detection and classification", based on SVM model.
