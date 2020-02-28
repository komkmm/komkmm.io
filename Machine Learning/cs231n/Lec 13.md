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
>![equation](https://latex.codecogs.com/gif.latex?p%28x%29%20%3D%20%5Cprod_%7Bn%7D%5E%7Bi%3D1%7Dp%28x_i%7Cx_1%2C%20...%2C%20x_%7Bi-1%7D%29)



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk1MzI1NjA3NywxMDI3NjAwODAwLDIwMD
kyNDE3NSwxNzkwMzIzNzBdfQ==
-->