# PanColorGAN
 Rethinking CNN-Based Pansharpening: Guided Colorization of Panchromatic Images via GANs.
 
# Abstract
Convolutional neural network (CNN)-based approaches have shown promising results in the pansharpening of the satellite images in recent years. However, they still exhibit limitations in producing high-quality pansharpening outputs. To that end, we propose a new self-supervised learning framework, where we treat pansharpening as a colorization problem, which brings an entirely novel perspective and solution to the problem compared with the existing methods that base their solution solely on producing a super-resolution version of the multispectral image. Whereas the CNN-based methods provide a reduced-resolution panchromatic image as the input to their model along with the reduced-resolution multispectral images and, hence, learn to increase their resolution together, we instead provide the grayscale transformed multispectral image as the input and train our model to learn the colorization of the grayscale input. We further address the fixed downscale ratio assumption during training, which does not generalize well to the full-resolution scenario. We introduce a noise injection into the training by randomly varying the downsampling ratios. Those two critical changes, along with the addition of adversarial training in the proposed PanColorization generative adversarial network (PanColorGAN) framework, help overcome the spatial-detail loss and blur problems that are observed in CNN-based pansharpening. The proposed approach outperforms the previous CNN-based and traditional methods, as demonstrated in our experiments.
 
# Paper
 If you find our work beneficial, consider citing the following paper:

F. Ozcelik, U. Alganci, E. Sertel and G. Unal, "Rethinking CNN-Based Pansharpening: Guided Colorization of Panchromatic Images via GANs," in IEEE Transactions on Geoscience and Remote Sensing, vol. 59, no. 4, pp. 3486-3501, April 2021, doi: 10.1109/TGRS.2020.3010441.


## Important Notes:
GAN training parts of the code are adapted from mrzhu-cool/pix2pix-pytorch [Github Link](https://github.com/mrzhu-cool/pix2pix-pytorch)

Metrics codes are adapted from different image quality assesment repos such as **sewar**

Pretrained Weights for PanColorGAN+RD can be found in the [Link](https://drive.google.com/file/d/1ONYO3m7zIlU1OW1et1DSYYpXxAaiBWpp/view?usp=sharing)

Google Colab Notebook for Pansharpening Demo [Colab](https://colab.research.google.com/drive/1N5lvyHLSbhbCOVmCtz5LL_9oGKuN1OUu)
