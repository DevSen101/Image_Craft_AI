# 🚀 ImageCraftAI

**ImageCraftAI** is a text-to-image generation application that converts natural language prompts into images using deep learning models. The project demonstrates the practical implementation of generative AI with an interactive web interface.

---

## 🔗 Google Colab

👉 [Link](https://colab.research.google.com/drive/1hAaM5Onsv5FJy7O3CdrVPP3sSNzSX8Q1?usp=sharing)

---

## 🧠 Core Functionality

The application uses a pre-trained **Stable Diffusion** model to generate images from text prompts.

### Workflow:

1. User provides a text prompt
2. Prompt is passed to the diffusion pipeline
3. Model generates latent representations
4. Image is decoded and returned as output
5. Displayed via web interface

---

## ⚙️ Tech Stack

* **Language:** Python
* **Model:** Stable Diffusion (runwayml/stable-diffusion-v1-5)
* **Framework:** Diffusers (Hugging Face)
* **Deep Learning:** PyTorch
* **Frontend/UI:** Gradio

---

## 🔍 Key Components

### 1. Model Pipeline

* Loaded using `StableDiffusionPipeline.from_pretrained()`
* Supports GPU acceleration using CUDA (if available)
* Uses `float16` for optimized performance on GPU

### 2. Image Generation Function

```python
def generate_image(prompt):
    image = pipe(prompt).images[0]
    return image
```

* Accepts text input
* Generates and returns image output

### 3. Interface Layer

* Built using Gradio
* Takes user input via textbox
* Displays generated image dynamically

---

## 📸 Screenshots

### 1️⃣ Introduction

<img width="1440" height="900" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/7093b703-4f8a-47e2-94f4-71e2bd543b58" />



---

### 2️⃣ Model Loading

<img width="1440" height="900" alt="Screenshot (108)" src="https://github.com/user-attachments/assets/d2990ff1-b2fa-4b57-af4d-5c92449ef4f0" />



---

### 3️⃣ Gradio Interface

<img width="1440" height="900" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/fbf19766-8194-4b9d-851e-aebe08e15bd7" />


---

## 🚀 Use Cases

* AI-based image generation
* Prompt engineering experiments
* Rapid prototyping of generative AI apps
* Educational demonstration of diffusion models

---

## 📌 Future Enhancements

* Add parameter tuning (steps, guidance scale)
* Image download & history
* API-based architecture (MERN integration)
* Model optimization for faster inference

---

## Author
Dev Kumar Sen
