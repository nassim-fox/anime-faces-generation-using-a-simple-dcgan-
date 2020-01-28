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

![Alt text] (/9999.png) 

### ref
[] Alec Radford, Luke Metz, and Soumith Chintala. Unsupervised representation learning with deep convolutional generative adversarial networks. CoRR,
abs/1511.06434, 2015.
