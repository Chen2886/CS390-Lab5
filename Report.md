# Report

### Info

Nuo (Tony) Chen, chen2886@purdue.edu

### Repo

https://github.com/Chen2886/CS390-Lab5

### Resources

 GANS slides from class

### Parts completed:

- [80] GANs.
  - [50] Complete the GAN to generate legible F-MNIST records. Generate from 3 classes.
  - [10] Use a convnet for the GAN networks.
  - [10] Save a plot of loss over training steps for each network.
  - [+~5] EC: Generate very detailed F-MNIST records (there is no metric for this, just do your best).
  - [+20] EC: Generate legible cifar records from 3 classes.

- [20] Report.

### Question

- Describe the discriminator and generator.
  - Both Discriminator is ANN and Generator is CNN.
  - Discriminator trys to separate fake images vs real images
  - Generator generates fake images from random noise
  - Generator is split up into 4 layer within the CNN using leaky relu as activation function, and discriminator is also split up into 4 layers but it uses ANN not CNNs. Discriminator flattens then uses leaky relu activation function
- Why do we sometimes need to train the discriminator and generator different amounts?
  - If they are different, one can make smaller steps and the other one can make bigger steps.

### Hyperparamaters

- Activation Function: Leaky Relu, Alpha = 0.2
- Batch Normalization, Momentum = 0.8
- Epochs: 40000
- Learning Rate: 0.0002

### Plot

![Sandal Gen](/Users/chen2886/Library/Mobile Documents/com~apple~CloudDocs/Sandal Gen.png)

![Sandal Dis](/Users/chen2886/Library/Mobile Documents/com~apple~CloudDocs/Sandal Dis.png)

![Coat Gen](/Users/chen2886/Library/Mobile Documents/com~apple~CloudDocs/Coat Gen.png)

![Coat Dis](/Users/chen2886/Library/Mobile Documents/com~apple~CloudDocs/Coat Dis.png)

![image-20210331214834742](/Users/chen2886/Library/Application Support/typora-user-images/image-20210331214834742.png)

![image-20210331214827003](/Users/chen2886/Library/Application Support/typora-user-images/image-20210331214827003.png)



### Pictures

Pictures are included in git repo, too much for here