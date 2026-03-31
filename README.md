# 🧠 Fashion MNIST Image Classification with PyTorch

This project focuses on building, training, and evaluating deep learning models for image classification using the FashionMNIST dataset. It explores how different neural network architectures perform on the same task, progressing from a simple linear model to a more advanced Convolutional Neural Network (CNN).

---

## 📌 Project Motivation

Image classification is a fundamental problem in computer vision. This project was designed to gain hands-on experience with:

- Designing neural network architectures
- Understanding the impact of non-linearity
- Leveraging convolutional layers for spatial feature extraction
- Building reusable training and evaluation pipelines

By comparing multiple models, this project highlights why deeper architectures like CNNs are more effective for image-based tasks.

---

## 🗂️ Dataset

The project uses the **FashionMNIST dataset**, which contains:
- 60,000 training images
- 10,000 test images
- 10 classes of clothing items (e.g., T-shirt, sneaker, bag)

Each image is a grayscale 28×28 pixel image.

---

## 🏗️ Models Implemented

### 🔹 Model 0: Linear Baseline
- Flattened image input
- Single linear layer
- No non-linearity  
➡️ Serves as a baseline for comparison

---

### 🔹 Model 1: Multilayer Perceptron (MLP)
- Fully connected layers
- ReLU activation functions  
➡️ Introduces non-linearity to improve learning capacity

---

### 🔹 Model 2: Convolutional Neural Network (CNN)
- Convolutional layers for feature extraction
- ReLU activations
- MaxPooling layers for downsampling
- Fully connected classification layer  

➡️ Captures spatial patterns in images, leading to better performance

---

## ⚙️ Training Pipeline

The models were trained using a structured pipeline:

- **Loss Function:** CrossEntropyLoss  
- **Optimizer:** Stochastic Gradient Descent (SGD)  
- **Batch Processing:** DataLoader for efficient mini-batch training  
- **Epoch-based training loop** with:
  - Forward pass
  - Loss computation
  - Backpropagation
  - Parameter updates  

---

## 📊 Evaluation & Metrics

Each model was evaluated using:

- **Accuracy** (classification performance)
- **Loss values** (training and test)
- **Confusion Matrix** for detailed class-wise analysis

The evaluation pipeline ensures consistency across all models for fair comparison.

---

## 🔍 Results & Insights

- The **linear model** performed the worst due to its inability to capture complex patterns.
- The **MLP model** improved performance by introducing non-linearity.
- The **CNN model achieved the best results**, demonstrating the importance of spatial feature extraction in image classification.

This confirms that convolutional architectures are more suitable for computer vision tasks.

---

## 🔮 Predictions & Visualization

The project includes:
- Random sample predictions from the test dataset
- Visualization of predicted vs true labels
- Color-coded outputs for easy interpretation
- Confusion matrix visualization to identify misclassifications

---

## 💾 Model Persistence

The best-performing model (CNN) was:
- Saved using `state_dict()`
- Reloaded into a new model instance
- Evaluated to confirm consistent performance

This step demonstrates how trained models can be reused for inference or deployment.

---

## 🛠️ Technologies Used

- Python  
- PyTorch  
- Torchvision  
- NumPy  
- Matplotlib  

---

## 🚀 Future Improvements

- Hyperparameter tuning (learning rate, batch size, epochs)
- Experimenting with deeper CNN architectures
- Adding dropout and regularization techniques
- Deploying the model as a web application
- Integrating real-time image input for predictions

---

## 📌 Key Takeaways

- Model architecture significantly impacts performance
- CNNs outperform fully connected networks in image tasks
- Structured training and evaluation pipelines improve reproducibility
- Visualization tools help in understanding model behavior

---

## 👨‍💻 Author

Computer Engineering graduate passionate about:
- Machine Learning & AI  
- Embedded Systems  
- Robotics  

---

⭐ If you find this project useful, feel free to star the repository!
