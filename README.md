# VAE study for MNIST

This repo contains code used for the results presented in my [Thinking AIoud blogpost](https://thinking-ai-aloud.blogspot.com/2020/11/variational-autoencoders-vae-hands-on.html).

The architecture used is a simple FFNN:

![architecture](media/mnist_vae.png)

Using a **2D latent space**, we are able to visualize it without distortions from dimensionality reduction:

![latent](media/train_latent_space.png)

Using such a VAE to **reconstruct** inputs results in somewhat blurry results:

![rec](media/vae2_reconstructions.png)

The result was the same while using the decoder as a generator:

![gen](media/vae2_samples.png)

However, that's where the **Conditional VAE** comes to the rescue:

![cvae](media/9cvaegrid.png)
