---
title: Acne Detection AI 🔥

short_description: Acne Segmentation & Severity Classification
---

# 🧠 Acne Detection & Classification with Deep Learning

![banner](https://huggingface.co/spaces/RihemXX/Acnes/resolve/main/images/output1.png) <!-- You can upload a real image here -->

This application demonstrates a powerful **AI-driven pipeline** for **acne detection, segmentation**, and **severity classification**, combining:

- A **UNet-based CNN** for precise acne lesion segmentation (pixel-wise accuracy ≈ **96–98%**)
- A **transformer-based classifier** (fine-tuned Vision Transformer) for grading severity based on dermatological standards

Try it by uploading a face image.  
It will return:
✅ a **visual overlay** showing detected acne regions  
✅ a **severity label** (from clear skin to very severe acne)

---

## 🧪 Model Architecture

### 🔹 Segmentation Model
- Architecture: `UNet` with `ResNet34` backbone (from [smp](https://github.com/qubvel/segmentation_models.pytorch))
- Optimized for: Binary mask prediction of acne regions
- Trained on: Annotated dermatological datasets
- Accuracy: **Pixel Accuracy ≈ 98%**, **IoU ≈ 91%**

### 🔹 Classification Model
- Architecture: Vision Transformer (ViT)
- Source: [`imfarzanansari/skintelligent-acne`](https://huggingface.co/imfarzanansari/skintelligent-acne)
- Labels: From `Level -1 (Clear)` to `Level 4 (Very Severe Acne)`
- Input: Facial image
- Output: Severity level + confidence score

---

## 📈 Example Output

| Input Image | Segmentation Overlay | Acne Level |
|-------------|----------------------|------------|
| ![input](https://huggingface.co/spaces/RihemXX/Acnes/resolve/main/images/image.png) | ![overlay](https://huggingface.co/spaces/RihemXX/Acnes/resolve/main/images/output.png) | Level 2: Moderate Acne |

---

## 💡 Use Cases
- Dermatology research and screening
- Skincare and cosmetic product testing
- Automated health monitoring platforms

---

## 🧩 Tech Stack
- `PyTorch`, `Segmentation Models PyTorch`
- `Transformers` by Hugging Face
- `Albumentations` for fast preprocessing
- `OpenCV`, `Gradio` for live interface




## 🤖 Try it now!

Click below and upload a photo to get real-time predictions:
[https://huggingface.co/spaces/RihemXX/Acnes](https://huggingface.co/spaces/RihemXX/Acnes)

Check out the configuration reference at [https://huggingface.co/docs/hub/spaces-config-reference](https://huggingface.co/docs/hub/spaces-config-reference)
