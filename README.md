# 🎨 AI Neural Style Transfer (AdaIN)

> **A production-ready Generative AI application that performs real-time artistic style transfer using Adaptive Instance Normalization (AdaIN), a pre-trained VGG-19 CNN, and perceptual loss optimization.**

![Python](https://img.shields.io/badge/Python-3.12-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![Generative AI](https://img.shields.io/badge/AI-Generative%20AI-red)
![CNN](https://img.shields.io/badge/CNN-VGG19-green)
![AdaIN](https://img.shields.io/badge/Style%20Transfer-AdaIN-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

# 📖 Overview

**AI Neural Style Transfer (AdaIN)** is a Generative AI application that transforms ordinary photographs into artistic images by combining the **content of one image** with the **style of another**. The project implements **Adaptive Instance Normalization (AdaIN)** with a **pre-trained VGG-19 convolutional neural network** to disentangle and recombine content and style features, enabling high-quality image stylization in real time.

The project showcases practical applications of **Transfer Learning**, **Deep Convolutional Neural Networks**, **Feature Embedding**, **Perceptual Loss Optimization**, and **Generative AI**, while demonstrating modern computer vision engineering practices.

---

# ✨ Features

- 🎨 Real-time artistic style transfer
- 🧠 Adaptive Instance Normalization (AdaIN)
- 🖼️ Content and style image fusion
- 🏛️ Pre-trained VGG-19 feature extraction
- ⚡ High-quality image stylization
- 📊 Perceptual loss optimization
- 🔄 Transfer learning pipeline
- 🧩 Modular architecture
- 🚀 Fast inference
- 📈 Easily extensible for additional style transfer models

---

# 📸 Demo

### Content Image

```
assets/demo/content.jpg
```

↓

### Style Image

```
assets/demo/style.jpg
```

↓

### Stylized Output

```
assets/demo/output.jpg
```

---

# 🏗 System Architecture

```text
             Content Image
                    │
                    ▼
             VGG-19 Encoder
                    │
                    │
                    ├──────────────┐
                    │              │
                    ▼              ▼
         Content Features     Style Features
                    ▲              ▲
                    │              │
             VGG-19 Encoder        │
                    │              │
                    ▼              │
               Style Image─────────┘
                    │
                    ▼
 Adaptive Instance Normalization (AdaIN)
                    │
                    ▼
            Feature Fusion
                    │
                    ▼
          Decoder Network
                    │
                    ▼
          Stylized Output Image
```

---

# 📂 Repository Structure

```text
ai-neural-style-transfer/
│
├── src/
│   ├── app/
│   ├── models/
│   ├── adain/
│   ├── feature_extractor/
│   ├── decoder/
│   ├── preprocessing/
│   ├── inference/
│   ├── losses/
│   ├── utils/
│   └── main.py
│
├── models/
│   ├── vgg19_weights/
│   └── trained_decoder/
│
├── datasets/
│   ├── content_images/
│   └── style_images/
│
├── assets/
│   ├── demo/
│   ├── screenshots/
│   └── architecture/
│
├── docs/
│   ├── Architecture.md
│   ├── Learnings.md
│   ├── Challenges.md
│   ├── Deployment.md
│   └── Future_Work.md
│
├── notebooks/
│
├── configs/
│
├── scripts/
│
├── tests/
│
├── .github/
│   └── workflows/
│
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

---

# ⚙️ Technology Stack

| Category | Technologies |
|-----------|--------------|
| Programming Language | Python |
| Deep Learning Framework | TensorFlow |
| CNN Backbone | VGG-19 |
| Transfer Learning | Pre-trained ImageNet Weights |
| Style Transfer | Adaptive Instance Normalization (AdaIN) |
| Image Processing | OpenCV / Pillow |
| Scientific Computing | NumPy |
| Visualization | Matplotlib |
| Version Control | Git & GitHub |

---

# 🧠 Generative AI Pipeline

```text
Content Image
       │
       ▼
Image Preprocessing
       │
       ▼
VGG-19 Feature Extraction
       │
       ▼
Content Feature Maps
       │
       ▼
AdaIN Feature Normalization
       ▲
       │
Style Feature Maps
       ▲
       │
Style Image
       │
       ▼
Feature Fusion
       │
       ▼
Decoder Network
       │
       ▼
Stylized Image
```

---

# 🔬 Core Concepts

- Adaptive Instance Normalization (AdaIN)
- Transfer Learning
- Deep Convolutional Neural Networks
- Feature Embeddings
- Content Representation
- Style Representation
- Perceptual Learning
- Feature Normalization
- Image-to-Image Translation

---

# 📉 Loss Functions

The model optimizes multiple objectives simultaneously:

- **Content Loss** – Preserves the structural content of the original image.
- **Style Loss** – Matches artistic style using feature statistics.
- **Perceptual Loss** – Ensures visually coherent outputs through deep feature comparison.
- **Total Variation Loss** – Produces smoother, artifact-free stylized images.

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/ai-neural-style-transfer.git
```

Navigate into the project

```bash
cd ai-neural-style-transfer
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Usage

Run the application

```bash
python src/main.py
```

Example

```bash
python src/main.py \
    --content assets/demo/content.jpg \
    --style assets/demo/style.jpg
```

The application will:

- Load the content image
- Load the style reference
- Extract deep features using VGG-19
- Apply AdaIN feature normalization
- Generate the stylized output
- Save the generated image

---

# 📊 Model Highlights

- Real-time style transfer
- Transfer learning with VGG-19
- High-fidelity artistic image generation
- Lightweight inference pipeline
- Modular deep learning architecture
- Extensible to multiple style transfer techniques

---

# 📚 Learning Outcomes

This project strengthened practical knowledge of:

- Generative AI fundamentals
- Neural Style Transfer
- Adaptive Instance Normalization
- Transfer Learning
- CNN feature extraction
- Feature-space manipulation
- Perceptual learning
- Deep image representations
- TensorFlow model development
- Production-ready deep learning pipelines

---

# ⚠️ Challenges Solved

- Separating content and style representations
- Preserving image structure during stylization
- Balancing multiple perceptual loss functions
- Optimizing inference speed
- Maintaining output quality across diverse artistic styles
- Efficient memory management for large images
- Designing a modular and scalable architecture

---

# 🛣 Roadmap

- [x] AdaIN Style Transfer
- [x] VGG-19 Feature Extraction
- [x] Perceptual Loss Optimization
- [x] High-Quality Image Stylization
- [ ] Multiple Artistic Style Blending
- [ ] Batch Image Stylization
- [ ] Video Style Transfer
- [ ] ONNX Export
- [ ] TensorRT Optimization
- [ ] Docker Deployment
- [ ] Streamlit Web Interface
- [ ] Diffusion Model Comparison

---

# 🤝 Contributing

Contributions are welcome.

Feel free to fork the repository, create a feature branch, and submit a pull request to improve the project.

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

**Abhishek Ojha**

AI • Generative AI • Deep Learning • Computer Vision • Transfer Learning

⭐ If you found this project helpful, consider giving it a **Star** on GitHub!
