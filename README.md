# anime-faces-generation-using-a-simple-dcgan-

## dataset
anime face dataset by Mckinsey666 : https://github.com/Mckinsey666/Anime-Face-Dataset
contains 63632 high-quality anime face

## model 
### DCGAN
DCGANs are generative models designed from GANs, made from conv-layers with no maxpooling. Downsampling is made using only strides and uses transposed convolutions for upsampling. 

- Replace all max pooling with convolutional stride
- Use transposed convolution for upsampling.
- Eliminate fully connected layers.
- Use Batch normalization except the output layer for the generator and the input layer of the discriminator.
- Use ReLU in the generator except for the output which uses tanh.
- Use LeakyReLU in the discriminator.

### intermediate result
this result is given at the 9999 epoch which is still to early to get clear results. It can be optimized, for example a more robust model can be used as descriminator. 

<img src="https://raw.githubusercontent.com/nassim-fox/anime-faces-generation-using-a-simple-dcgan-/master/9999.png" width="300">

### ref
[] Alec Radford, Luke Metz, and Soumith Chintala. Unsupervised representation learning with deep convolutional generative adversarial networks. CoRR,
abs/1511.06434, 2015.
