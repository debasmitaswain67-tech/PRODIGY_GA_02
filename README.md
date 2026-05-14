# 🎨 DALL-E Mini Image Generator

### Generate Square (1:1) Digital Art from a Text Prompt using DALL-E Mini

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QClJkH0fHO1bvhix7Vqb3fb4_uHOcrxe#scrollTo=_-0nMR4EX0Jj)

---

## 📌 Overview

This project uses **DALL-E Mini (MinDalle)** to generate square digital art images from a simple text prompt. Given any descriptive prompt, the model generates a **3×3 grid of images**, from which the best one can be selected and saved.

---

## 🚀 Features

- ✅ Text-to-image generation using DALL-E Mini
- ✅ Generates a 3×3 grid of square (1:1) images
- ✅ GPU-accelerated (CUDA supported)
- ✅ Saves both the full grid and the selected best image
- ✅ Configurable prompt, seed, and generation parameters

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `min-dalle` | Lightweight DALL-E Mini model |
| `PyTorch` | Deep learning backend |
| `CLIP` | Text-image alignment |
| `Pillow` | Image handling |
| `Matplotlib` | Visualization & saving output |

---

## ⚙️ Setup & Usage

### 1. Open in Google Colab
Click the badge above or use this link:
[DALL-E Mini Image Generator Task2 - Colab](https://colab.research.google.com/drive/1QClJkH0fHO1bvhix7Vqb3fb4_uHOcrxe#scrollTo=_-0nMR4EX0Jj)

### 2. Enable GPU Runtime
> Go to `Runtime → Change runtime type → Hardware accelerator → T4 GPU`

### 3. Run All Cells in Order

| Section | Description |
|---------|-------------|
| Section 1 | Verify GPU with `nvidia-smi` |
| Section 2 | Install all dependencies |
| Section 3 | Load DALL-E Mini model |
| Section 4 | Set your text prompt & generate images |

---

## 🖼️ Example Prompt

```python
TEXT_PROMPT = "a place with heavy rainfall, thunderstorm and lightning, digital art"
```

### Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| `NUM_IMAGES` | 9 | Total images in grid |
| `GRID_SIZE` | 3 | 3×3 grid layout |
| `SEED` | 42 | Change for different results |
| `SUPERCONDITION_FACTOR` | 16 | Higher = more prompt-faithful |
| `TOP_K` | 256 | Sampling diversity |

---

## 📁 Output Files

- `dalle_mini_grid.png` — Full 3×3 generation grid
- `selected_image.png` — Best selected square image

---

## 📚 References

- [min-dalle by Brett Kuprel](https://github.com/kuprel/min-dalle)
- [Original DALL-E Mini Colab](https://colab.research.google.com/github/robgon-art/e-dall-e/blob/main/DALL_E_Mini_Image_Generator.ipynb)

---

## 👩‍💻 Author

**debasmitaswain67-tech**
