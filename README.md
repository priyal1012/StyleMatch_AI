

<div align="center">

# 👔 StyleMatch AI

### Deep Learning Powered Visual Fashion Recommendation System

<p align="center">
Transforming Visual Similarity Search into Intelligent Fashion Discovery
</p>

<p align="center">

![Python](https://img.shields.io/badge/Python-3.7-blue?style=for-the-badge\&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge\&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge\&logo=keras)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge\&logo=opencv)
![Streamlit](https://img.shields.io/badge/Streamlit-Web_App-FF4B4B?style=for-the-badge\&logo=streamlit)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-Machine_Learning-F7931E?style=for-the-badge\&logo=scikitlearn)

</p>

*A Deep Learning-based Fashion Recommendation Engine capable of retrieving visually similar products through high-dimensional feature representation and similarity-based image retrieval.*

</div>



# 📌 Overview

StyleMatch AI is a **Content-Based Fashion Recommendation System** that intelligently retrieves visually similar fashion products using **Deep Learning**, **Transfer Learning**, and **Feature Embedding** techniques.

Instead of depending upon textual descriptions, manually assigned product tags, or metadata, the system performs recommendation entirely through **visual understanding**. An uploaded fashion image is analyzed by a pre-trained deep convolutional neural network, transformed into a compact numerical representation, and compared against thousands of product images stored in the database to retrieve the most visually relevant recommendations.

The system supports multiple fashion categories including:

* 👕 T-Shirts
* 👔 Shirts
* 👖 Pants
* 👟 Shoes
* ⌚ Watches
* 👗 Sarees
* 👜 Fashion Accessories

Once an image is uploaded, the recommendation engine extracts its visual representation using a **pre-trained ResNet50 model**, generates a **2048-dimensional feature embedding**, compares it against feature embeddings of every product present in the dataset, and finally returns the **Top-5 most visually similar products**.



# ✨ Features

* 📷 Image-Based Fashion Recommendation
* 🧠 Deep Feature Extraction using ResNet50
* 🚀 Transfer Learning with ImageNet Pre-trained Weights
* 📊 High-Dimensional Feature Embedding Generation
* 🔍 Similarity-Based Product Retrieval
* ⚡ K-Nearest Neighbour Search
* 🎯 Top-5 Visual Product Recommendation
* 🌐 Interactive Streamlit Web Application
* 📂 Large Fashion Image Repository
* 💻 User-Friendly Interface



# 🎯 Problem Statement

Traditional recommendation systems generally rely on product descriptions, manually assigned categories, keywords, or purchase history.

However, users often possess only an image of a fashion product without knowing its brand, category, or textual description.

StyleMatch AI addresses this challenge by implementing an intelligent visual recommendation pipeline capable of identifying aesthetically similar fashion products solely from their visual characteristics.

Instead of comparing raw pixels, the system learns rich semantic representations of images and performs recommendation through feature similarity, enabling efficient and accurate visual product discovery.



# 🏗️ Project Architecture

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/d6a7a2b0-1cdc-46f0-80fe-5ef88222eb44" />


# 🛠️ Technology Stack

| Category                | Technology   |
| ----------------------- | ------------ |
| Programming Language    | Python 3.7   |
| Deep Learning Framework | TensorFlow   |
| Deep Learning API       | Keras        |
| Transfer Learning       | ResNet50     |
| Pre-trained Weights     | ImageNet     |
| Image Processing        | OpenCV       |
| Numerical Computing     | NumPy        |
| Machine Learning        | Scikit-Learn |
| Web Framework           | Streamlit    |



# 🧠 Methodology

The recommendation pipeline consists of multiple sequential stages designed to transform raw fashion images into highly informative numerical representations capable of capturing complex visual semantics.

### 1. Image Upload

The user uploads an image of a fashion product through the Streamlit web interface.



### 2. Image Preprocessing

The uploaded image is resized to **224 × 224** pixels and preprocessed to match the input format expected by the pre-trained ResNet50 architecture.



### 3. Deep Feature Extraction

Instead of training a convolutional neural network from scratch, the project utilizes a **pre-trained ResNet50** model that has already learned rich visual representations from the ImageNet dataset.

The original classification layer is removed, allowing the network to function purely as a high-level feature extractor.

---

### 4. Global Max Pooling

A Global Max Pooling layer converts convolutional feature maps into a compact **2048-dimensional feature vector**, preserving the most discriminative visual information while significantly reducing computational complexity.

---

### 5. Feature Normalization

The generated embedding vector is normalized to ensure consistent numerical scaling across all product representations before similarity computation.

---

### 6. Similarity Search

The normalized feature embedding of the uploaded image is compared against feature embeddings generated for every image present within the product database.

Similarity computation is performed using the **K-Nearest Neighbour algorithm**, enabling efficient retrieval of visually related products.

---

### 7. Recommendation Generation

The five products exhibiting the highest visual similarity are retrieved and presented to the user as personalized recommendations.

---

# 📂 Project Structure

```text
StyleMatch_AI/
│
├── images/
├── uploads/
├── app.py
├── feature_extraction.py
├── embeddings.pkl
├── filenames.pkl
├── requirements.txt
└── README.md
```

---

# 💡 Why Transfer Learning?

Training a deep convolutional neural network from scratch requires enormous computational resources, extensive datasets, and significant training time.

Instead, this project leverages **Transfer Learning** by utilizing a ResNet50 model already trained on the ImageNet dataset.

This approach enables powerful feature extraction without requiring expensive end-to-end model training while achieving highly informative visual representations.

---

# 🌟 Applications

* Fashion Recommendation Systems
* E-Commerce Platforms
* Visual Product Search
* Reverse Image Search
* Apparel Discovery Systems
* Fashion Retail Analytics
* Product Similarity Retrieval

---

# 📈 Future Improvements

* Multi-image recommendation
* Personalized recommendation pipeline
* Faster large-scale similarity retrieval
* Enhanced user interface
* Larger fashion product repository
* Support for additional product categories

---

# 👨‍💻 Author

**Priyal**

---

⭐ **If you found this project useful, consider giving it a Star!**



