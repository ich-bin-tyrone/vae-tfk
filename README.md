# 🎨 VAE-Based Image Interpolator  

This project implements a **Variational Autoencoder (VAE)** based image interpolator. It generates new "in-between" images by interpolating between two different image classes using a weighted combination of their latent space distributions.  

---

## 🚀 Features  
✅ **Variational Autoencoder (VAE)** for learning latent representations  
✅ **Latent Space Interpolation** for smooth class transitions  
✅ **Customizable Weighting** to control the class influence  
✅ **Scalable** for different datasets and resolutions  

---

## 📦 Installation  
Ensure you have Python and the necessary dependencies installed.  

---

## 🔧 How to Use  
### **1️⃣ Train the VAE Model**  
Train the model on your dataset:  
```sh
python model.ipynb --dataset path/to/dataset
```

### **2️⃣ Perform Interpolation**  
Generate interpolated images between two classes:  
```sh
python interpolate.py --class1 label1 --class2 label2 --alpha 0.5
```
- `alpha`: Controls the weighting between the two classes (`0.0 = full class1`, `1.0 = full class2`).  

---

## 🎯 Example  
Suppose you have a dataset of handwritten digits (MNIST). You can interpolate between `0` and `1` as follows:  
```sh
python interpolate.py --class1 0 --class2 1 --alpha 0.5
```
This will generate an image that blends digit `0` and digit `1`.  

---

## 📂 Folder Structure  
```
├── train.py               # Training script  
├── interpolate.py         # Interpolation script  
├── models/               # Model checkpoints  
├── datasets/             # Dataset storage  
├── requirements.txt      # Dependencies  
└── README.md             # Project documentation  
```

---

## 💡 Future Improvements  
✨ Implement different distance metrics for interpolation  
✨ Extend to Conditional VAE (cVAE) for better class control  
✨ Test on high-resolution datasets  

---

## 📜 License  
This project is licensed under the MIT License.  
