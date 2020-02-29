# Supervised vs Unsupervised Learning 
## Supervised Learning
* Data : (x, y) x is data, y is label
* Goal : Learn a *function* to map x -> y
* Examples : Classification, regression, object detection, semantic segmentation, image captioning, etc.

## Unsupervised Learning
* Data : x. just data, no labels
* Goal : Learn some underlying hidden *structure* of the data
* Examples : Clustering, dimensionality reduction, feature learning, density estimation, etc.


# Generative Models(unsupervised)
> Given training data, generate new samples from same distribution
* approach
	- Explicit density estimation : explicitly define and solve for p_model(x)
	- Implicit density estimation : learn model that can sample from p_model(x) w/o explicitly defining it

* Taxonomy
![intro](/img/intro.png)

this class will discuss about 3 most popular types models
(PixelRNN/CNN, Variational Autoencoder(VAE), GAN)

## PixelRNN/CNN(Explicit density model)
> Fully visible belief network, 
> Use chain rule to decompose likelihood of an image x into product of 1-d distributions  

>![equation](https://latex.codecogs.com/gif.latex?%5C%5Cp%28x%29%20%3D%20%5Cprod_%7Bn%7D%5E%7Bi%3D1%7Dp%28x_i%7Cx_1%2C%20...%2C%20x_%7Bi-1%7D%29%5C%5C%20%5C%5Cp%28x%29%20%3A%20Likelihood%5C%2Cof%5C%2Cimage%5C%2C%20X%20%5C%5Cp%28x_i%7C%20...%29%20%3A%20Probability%5C%2Cof%5C%2C%27i%27th%5C%2Cpixel%5C%2Cvalue%5C%2Cgiven%5C%2Call%5C%2Cprevious%5C%2Cpixels)
* objective : maximize likelihood of training data

* Generate image pixels starting from corner using RNN(LSTM) or CNN

## Variational Autoencoder(VAE)
### Autoencoder(background)
> Unsupervised approach for learning a lower-dimensional feature representation from unlabeled training data
> 
* 



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxODUzOTU2NiwzNzU4NDM0MTAsLTE1NT
A0OTg4MCwyOTc4MDY5MDYsLTk1MzI1NjA3NywxMDI3NjAwODAw
LDIwMDkyNDE3NSwxNzkwMzIzNzBdfQ==
-->