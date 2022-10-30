# Variational Autoencoder (VAE) for Predicting Microstructure by Using Mechanical MNIST

## Goal
This repository consists of example code for the implementation of one of the common generative model architectures: Variational Autoencoder (VAE) for a material science problem. VAEs represent each datapoint as probability distribution and embedds the meanningful relations in low-dimensional latent space. These models can be used to perform inverse materials design, which means it is possible to predict structure or processing parameters for given target material properties.

In this materials design example, it was aimed to predict microstructure evolution, in both backward and forward, for a binary material system. Even though, the [Mechanical Dataset](https://github.com/elejeune11/Mechanical-MNIST-Cahn-Hilliard) was prepared by assuming the material had Neo-Hookean hyperelasticity material -unlike most alloys that have an elastoplasticity behavior, the methodology can be used for similar problems in different material systems.

## Methodology
When the model is trained with the dataset consisting of microstructure images of the material, the model extracts the most important features in each microstrcuture and represent these feature by its design space. This design space is actually known as "latent space" in computer science terminology. Model can extrapolate a known microstructure in backward and forward evolution by using the available information as in probability distribution form in the latent space.

The extrapolation in latent space was performed by randomly choosing microstructures and tailoring each latent space axis.

## How to use
To perform extrapolation, a random microstructure can be selected and by following the instructuctions in "" notebook, the chosen and extrapolated images can be visualized.

## Additional Notes

The code was written on Google Colab platform. Different installation of libraries or functions might be required to use the notebook in local machines.

This repository is expected to help students and researchers who would like to learn how to use deep learning and especially generative deep learning in material science. This implementation of generative model was done by non-computer scientist, so any contribution is welcome!


