# 🖼️ Stable Diffusion Image Generator

This project allows you to generate high-quality images from text prompts using Hugging Face's `diffusers` library and various pre-trained Stable Diffusion models.

---

## 📦 Features

- Support for multiple Stable Diffusion models via a dictionary.
- Easy-to-use CLI input with default parameters.
- Automatic device selection (GPU if available).
- Saves generated images with timestamped filenames.
- Visualizes results using Matplotlib.
- Resource cleanup to manage memory (especially on GPU).

---

## 🔧 Requirements

Install the required Python packages:

```bash
pip install diffusers transformers accelerate torch pillow tqdm
