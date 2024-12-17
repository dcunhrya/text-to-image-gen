# text-to-image-gen

We present models to perform text to image generation and image reconstruc-
tion using a conditional VAE (CVAE) trained on Fashion-MNIST for short-text
and COCO for long-text with a CLIP feature extractor. In total, three main ex-
periments were run. The first experiment involved short-text model architecture
investigation between fully connected and a convolutional CVAE, where the con-
volutional CVAE was found to have a lower MSE and higher SSIM and FID.
The second experiment tested long-text image generation and reconstruction on
images of size 64x64, 128x128, and 256x256. The third experiment tested con-
catenating versus adding the conditional input in the CVAE from the COCO anno-
tation using the features extracted by CLIP. Both conditioning methods resulted in
similar results for sizes of 64x64 and 128x128, but the concatenation conditioning
significantly outperformed the adding conditioning with 256x256 images.
