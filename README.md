# MNIST_Digit_classification_using_Neural_Networks_major_project

##  Overview
This project implements a **Neural Network** to classify handwritten digits (0–9) from the **MNIST dataset**. The model achieved **97.5% test accuracy**, exceeding the target of 90%, and successfully predicted a custom image of digit **3**.

##  Objectives
- Load and preprocess MNIST dataset  
- Build and train a neural network model  
- Evaluate performance using accuracy and confusion matrix  
- Test predictions on custom user-provided images  

##  Dataset
- **Source**: MNIST (60,000 training images, 10,000 test images)  
- **Image Size**: 28×28 grayscale  
- **Preprocessing**: Pixel normalization (0–1 range)  

##  Tools & Technologies
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- OpenCV (for custom image processing)  

##  Methodology
1. **Data Loading**: Imported MNIST dataset via `keras.datasets.mnist`.  
2. **Preprocessing**: Normalized pixel values, reshaped images.  
3. **Model Architecture**:  
   - Input Layer: Flatten (784 neurons)  
   - Hidden Layers: Dense (128 + 64 neurons, ReLU activation)  
   - Output Layer: Dense (10 neurons, Softmax activation)  
   - Loss: Sparse Categorical Crossentropy  
   - Optimizer: Adam  
4. **Training**: 5 epochs, achieving 98.8% training accuracy.  
5. **Evaluation**: Test accuracy of 97.5%, confusion matrix visualization.  
6. **Custom Prediction**: Processed `3-digit.PNG` using OpenCV, correctly predicted digit **3**.  

##  Results
| Metric              | Target   | Achieved | Status |
|---------------------|----------|----------|--------|
| Model Accuracy      | >90%     | 97.5%    |  Exceeded |
| Custom Prediction   | Correct  | Digit 3  |  Passed |

##  Key Takeaways
- Neural network achieved high accuracy and generalization.  
- Preprocessing (normalization) was crucial for convergence.  
- Custom image prediction validated real-world applicability.  

##  Future Scope
- Extend to **CNN architectures** for even higher accuracy.  
- Deploy as a **web app** for interactive digit recognition.  
- Integrate with handwriting recognition systems.  

