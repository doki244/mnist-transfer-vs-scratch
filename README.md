# MNIST Classification: CNN from Scratch vs. Fine-Tuned MobileNetV2

This project compares the performance of custom-designed CNN models versus a pre-trained MobileNetV2 model fine-tuned on the MNIST handwritten digit classification task.

## 📌 Project Goals
- Build and train two distinct CNN architectures from scratch using PyTorch.
- Track and compare training loss and accuracy on test data for each.
- Fine-tune MobileNetV2 (pre-trained on ImageNet) for MNIST.
- Visualize and analyze model performance.

---

## 🧠 Part 1: Custom CNN Architectures

- **Net1**: Simple architecture with two Conv layers + MaxPooling + 3 FC layers.
- **Net2**: Slightly deeper architecture with Dropout and different filter setup.

### 📊 Metrics
- Accuracy calculated on MNIST test set after each epoch.
- Loss and accuracy curves plotted to compare training dynamics.

---

## 🧠 Part 2: Transfer Learning with MobileNetV2

- Pre-trained MobileNetV2 loaded from `torchvision.models`.
- Adapted for grayscale MNIST by converting to 3-channel format and resizing to 224x224.
- Final fully connected layer replaced to output 10 classes.
- Fine-tuned on MNIST training set.

---

## 🛠️ Technologies Used

- Python, PyTorch
- torchvision, matplotlib, numpy
- MobileNetV2 (transfer learning)


