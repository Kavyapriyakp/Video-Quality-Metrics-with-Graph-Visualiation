# Video-Quality-Metrics-with-Graph-Visualiation

psnr	Peak signal-to-noise ratio (pSNR)
pSNR is derived from the mean square error, and indicates the ratio of the maximum pixel intensity to the power of the distortion. Like MSE, the pSNR metric is simple to calculate but might not align well with perceived quality. 

ssim	 Structural similarity (SSIM) index. The SSIM metric combines local image structure, luminance, and contrast into a single local quality score. In this metric, structures are patterns of pixel intensities, especially among neighboring pixels, after normalizing for luminance and contrast. Because the human visual system is good at perceiving structure, the SSIM quality metric agrees more closely with the subjective quality score. 

brisque	Blind/Referenceless Image Spatial Quality Evaluator (BRISQUE). A BRISQUE model is trained on a database of images with known distortions, and BRISQUE is limited to evaluating the quality of images with the same type of distortion. BRISQUE is opinion-aware, which means subjective quality scores accompany the training images. 

niqe	Natural Image Quality Evaluator (NIQE). Although a NIQE model is trained on a database of pristine images, NIQE can measure the quality of images with arbitrary distortion. NIQE is opinion-unaware, and does not use subjective quality scores. The tradeoff is that the NIQE score of an image might not correlate as well as the BRISQUE score with human perception of quality. 

piqe	Perception based Image Quality Evaluator (PIQE). The PIQE algorithm is opinion-unaware and unsupervised, which means it does not require a trained model. PIQE can measure the quality of images with arbitrary distortion and in most cases performs similar to NIQE. PIQE estimates block-wise distortion and measures the local variance of perceptibly distorted blocks to compute the quality score.
