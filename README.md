# MNIST Digit Generator

This project demonstrates the use of a Generative Adversarial Network (GAN) to generate handwritten digits similar to those found in the MNIST dataset. The MNIST dataset is a well-known dataset in the field of machine learning, consisting of 60,000 training images of handwritten digits from 0 to 9. The project is implemented using PyTorch.

## Project Structure
The project directory is structured as follows:

```
MNIST_DIGIT_GENERATOR/
│
├── models/
│   ├── mnist_generator.pth                       # Weights of MNIST Generator
│   └── mnist_discriminator.pth                   # Weights of MNIST Discriminator
│
├── notebooks/
│   ├── mnist_generator_training.ipynb            # Jupyter notebook for GAN Training
|   ├── mnist_generator_testing.ipynb             # Jupyter notebook for GAN Testing
│
└── README.md                                     # This README file
```

## Usage
### Training the GAN
To train the GAN, run the Jupyter notebook `mnist_generator_training.ipynb` located in the `notebooks/` directory. This notebook contains the implementation for training the GAN using the MNIST dataset and will save the models in the `models/` directory.

### Generating Images
To generate images, you can use pre-trained weights from this repository or train the GAN using `mnist_generator_training.ipynb` and save the weights. You can then load the saved generator model and create new handwritten digit images. This process can also be done within the Jupyter notebook using `mnist_generator_testing.ipynb`.

### Results
After training the GAN, you can evaluate its performance by generating images and comparing them to the original MNIST dataset. Use the Jupyter notebook `mnist_generator_testing.ipynb` to visualize and assess the quality of the generated digits. You can also adjust the training parameters to see how they affect the output quality. The results should showcase realistic handwritten digits, demonstrating the effectiveness of the GAN model.
