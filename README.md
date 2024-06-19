
# Image-Denoising-using-Deep-learning

## INRODUCTION

### What is Image Denoising ?
The images that are captured in the real world come with noises. These noises can appear due to many reasons such as electric signal instabilities, malfunctioning of camera sensors, poor lighting conditions, errors in data transmission over long distances, etc. This can degrade the captured image's quality and can cause loss of information as the original pixel values are replaced by random values due to noise. So, there is a need to remove these noises from images when it comes to low-level vision tasks and image processing. The process of removing such noises from images is known as Image Denoising. Image denoising techniques aim to restore an image to its original quality by reducing or removing the noise, while preserving the important features of the image.

### Deep Learning
A deep learning model is a neural network that is composed of multiple layers. The first layer is the input layer, which receives input data. The second layer is the hidden layer, which transforms the input data into a representation that can be used by the output layer. The output layer produces the desired output.

###Performance Metrics
**Peak Signal to Noise Ratio (PSNR)** - The term peak signal-to-noise ratio (PSNR) is an expression for the ratio between the maximum possible value (power) of a signal and the power of distorting noise that affects the quality of its representation.  Because many signals have a very wide dynamic range, (ratio between the largest and smallest possible values of a changeable quantity) the PSNR is usually expressed in terms of the logarithmic decibel scale. The higher the PSNR, the better the quality of the compressed image.

![Alt text](https://imgs.search.brave.com/RaSB2gP-JSH6-GRaQtoCcCQdE5NjAtJ3Q_FSuOk6wFk/rs:fit:860:0:0/g:ce/aHR0cHM6Ly93d3cu/cGFudGVjaHNvbHV0/aW9ucy5uZXQvd3At/Y29udGVudC91cGxv/YWRzLzIwMTMvMTEv/cHNuci1hbmQtbXNl/LnBuZw)
                         
### METHODOLOGIES USED
#### Results from AutoEncoder

### Building of Model-
![Alt text](https://i.ibb.co/S3Pp5VL/Auto-Encoder-Model.png)
 
### Model Fitting-
![Alt text](https://i.ibb.co/d4sG2b5/Auto-Encoder-Model-Fitting.png)
 
### Noising Factor-
![Alt text](https://i.ibb.co/L0DVwLk/Auto-Encoder-Noise-Factor.png)

### Predicted data-
![Alt text](https://i.ibb.co/2MZJ0kS/Auto-Encoder-Predicted-Data.png)

### Noised Testing data-
![Alt text](https://i.ibb.co/ZN9Y9Qt/Auto-Encoder-Testing-Data.png)

### Average PSNR value-
![Alt text](https://i.ibb.co/47zHkJy/Auto-Encoder-PSNR-AVERAGE.png)
 

### Zero DCE (Zero-Reference Deep Curve Estimation) –
Zero-Reference Deep Curve Estimation (Zero-DCE) formulates light enhancement as a task of image-specific curve estimation with a deep network. This method trains a lightweight deep network, DCE-Net, to estimate pixel-wise and high-order curves for dynamic range adjustment of a given image. The curve estimation is specially designed, considering pixel value range, monotonicity, and differentiability. Zero-DCE is appealing in its relaxed assumption on reference images, i.e., it does not require any paired or unpaired data during training. This is achieved through a set of carefully formulated non-reference loss functions, which implicitly measure the enhancement quality and drive the learning of the network. This method is efficient as image enhancement can be achieved by an intuitive and simple nonlinear curve mapping. A Deep Curve Estimation Network (DCE-Net) is devised to estimate a set of best-fitting Light-Enhancement curves (LE-curves) given an input image. The framework then maps all pixels of the input’s RGB channels by applying the curves iteratively for obtaining the final enhanced image.
 

![Alt text](https://i.ibb.co/QXXpXH7/DCE-Explain2.png)

![Alt text](https://i.ibb.co/6tyqvV7/DCE-Explain.png)

### Building of Model-
![Alt text](https://i.ibb.co/RypqcB4/DCE-Model.png)

### Testing data-
![Alt text](https://i.ibb.co/JpGXsJV/DCE-Dataset.png)

### Training and Testing of data-
![Alt text](https://i.ibb.co/zSFRNVz/DCE-Training-and-Testing.png)

### PSNR value-
![Alt text](https://i.ibb.co/0fSjMrR/DCE-PSNR.png)
 


### REFERENCES
1.	https://medium.com/analytics-vidhya/noise-removal-in-images-using-deep-learning-models-3972544372d2
2.	https://www.youtube.com/watch?v=ggJhpgXK6E0
3.	https://github.com/chintan1995/Image-Denoising-using-Deep-Learning/tree/main
4.	https://medium.com/analytics-vidhya/image-denoising-using-deep-learning-dc2b19a3fd54
