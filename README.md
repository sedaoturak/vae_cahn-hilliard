# Conditional Variational Autoencoder (cVAE) for Materials Design with Tailored Mechanical Properties

This repository consists of example code for the implementation of one of the common generative model architectures: conditional Variational Autoencoders (cVAE). VAEs represent each datapoint as probability distribution and embedds the meanningful relations in low-dimensional latent space. These models can be used to perform inverse materials design, which means it is possible to predict structure ot processing parameters for given target material properties.

For a materials design problem, when the model is trained with a dataset consisting of structure-property relationships of a material, the model unreveals how structural features result in specific material properties. The model extracts the most important features in strcutural data and uses them as the coordinates of its design space. This design space is actually the "latent space" in computer science terminology. In cVAE, material properties are defined as conditions in the model so that model can map this information in the design space by pairing with conditions. To use the model for inverse materials design, target material property is given to the model as condition and model finds the corresponding structure in its design space by using the available information as in probability distribution form.

The dataset in this example is the Mechanical MNIST dataset created from original MNIST dataset. -for more information, visit [this repository](https://github.com/elejeune11/Mechanical-MNIST).

Additionally, the notebook consists of latent space exploration with sampling, interpolation in latent space and in condition practices.

The code was written on Google Colab platform. Different installation of libraries or functions might be required to use the notebook in local machines.

This repository is expected to help students and researchers who would like to learn how to use deep learning and especially generative deep learning in material science. This implementation of generative model was done by non-computer scientist, so any contribution is welcome!

## Playing with the code
The notebook can be ran directly on Colab. To perform inverse design, the condition must be given to the Decoder part oof the model in "Inverse Design" section in the notebook.
