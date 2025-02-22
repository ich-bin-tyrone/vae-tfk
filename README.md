# VAE-Based Image Interpolator 🚀

## Overview 🖼️
This project implements a Variational Autoencoder (VAE) based image interpolator. The model can generate new "in-between" images by interpolating between two different image classes. This is achieved by sampling from the latent space using a weighted combination of the distributions of the two classes.

## Features ✨
- **Variational Autoencoder (VAE)** for learning latent representations.
- **Latent Space Interpolation** to generate smooth transitions between two image classes.
- **Customizable Weighting** to control the influence of each class in the interpolation.
- **Scalability** to different datasets and image resolutions.

## Installation ⚙️
Ensure you have Python and the necessary dependencies installed:
```sh
pip install -r requirements.txt
```

## Usage 🚀
1. Train the VAE on your dataset:
   ```sh
   python train.py --dataset path/to/dataset
   ```
2. Perform interpolation between two classes:
   ```sh
   python interpolate.py --class1 label1 --class2 label2 --alpha 0.5
   ```
   - `alpha` controls the weighting between the two classes (0.0 = full class1, 1.0 = full class2).

## Example 🏆
Suppose you have a dataset of handwritten digits (MNIST). You can interpolate between `0` and `1` as follows:
```sh
python interpolate.py --class1 0 --class2 1 --alpha 0.5
```
This will generate an image that is an approximate blend of digit `0` and digit `1`.

## Dependencies 📦
- Python 3.x
- TensorFlow/PyTorch
- NumPy
- Matplotlib

## Future Improvements 🚀
- Implementing different distance metrics for interpolation.
- Extending to conditional VAE (cVAE) for better class control.
- Testing on high-resolution datasets.

## License 📜
This project is licensed under the MIT License.

