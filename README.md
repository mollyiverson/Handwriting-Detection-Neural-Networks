# Handwriting Detection Using Neural Networks  

### **Team Members**  
- Molly Iverson
- Caitlin Graves
- Chandler Juego

---

## **Project Overview**  
Handwriting detection remains a challenging task due to variations in writing styles, sizes, and orientations. This project evaluates and compares three neural network models—Traditional Neural Network, Convolutional Neural Network (CNN), and Capsule Neural Network (CapsNet)—to determine their effectiveness in identifying handwritten digits.  

---

## **Datasets**  
**Source 1:** [MNIST Dataset](https://www.kaggle.com/datasets/hojjatk/mnist-dataset)  
**Description:**  
- 28x28 pixel grayscale images of handwritten digits (0-9).  
- **Training Set:** 60,000 images  
- **Test Set:** 10,000 images

**Source 2:** [Rotated MNIST Dataset](https://www.kaggle.com/code/teenakunsoth/mnist-rotated)  
**Description:**  
- 28x28 pixel grayscale images of handwritten digits (0-9) rotated at random degrees.  
- **Training Set:** 50,000 images  
- **Test Set:** 12,000 images  

The MNIST dataset provides a standardized way to test and evaluate handwriting detection algorithms.  

---

## **Algorithms**  

### 1. **Traditional Neural Network (NN)**  
- A simple feedforward neural network.  
- Does not consider spatial relationships in images.  
- Least computationally expensive but also least accurate.  

### 2. **Convolutional Neural Network (CNN)**  
- Leverages convolutional layers to detect spatial patterns like edges and shapes.  
- Achieves high accuracy by learning hierarchical features.  
- More computationally efficient than CapsNet but less robust to variations in orientation and style.  

### 3. **Capsule Neural Network (CapsNet)**  
- Uses capsules to model spatial hierarchies and dynamic routing to learn feature relationships.  
- Excels at handling variations in writing styles, orientations, and distortions.  
- High accuracy but computationally expensive.  

---

## **Results**  

| **Model**    | **Accuracy** | **Strengths**                           | **Weaknesses**                          |  
|--------------|--------------|-----------------------------------------|-----------------------------------------|  
| NN           | 96.54%       | Fast and computationally cheap          | Poor spatial understanding              |  
| CNN          | 98.78%       | Efficient and accurate                  | Limited robustness to spatial variations|  
| CapsNet      | 99.3%        | Robust to variations and distortions    | High computational cost                 |  

---

## Acknowledgments
[MNIST Dataset](https://yann.lecun.com/exdb/mnist/) by Yann LeCun, Corinna Cortes, and Christopher J.C. Burges.
