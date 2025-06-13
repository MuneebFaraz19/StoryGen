# 🖼️ Visual Story Generator: Turning Images into Stories

**"A picture speaks a thousand words" — and now, literally.**
**Colab link:** https://colab.research.google.com/drive/1PiiQDStaY9g0i4ekMLo2J1yhIKZnuJvb?usp=sharing

This project generates **context-aware stories** from input images by combining deep computer vision and natural language generation. It’s designed to assist **writers, creatives, and storytellers** in turning visual content into rich narratives.

---

## 🚀 Project Highlights

- 🧠 **Hybrid Deep Learning Pipeline**  
  Combines a **ResNet-based image encoder** with a **GPT-2 language model** to produce full stories from images.

- 📸 **Input**: A single image  
- 📜 **Output**: A short story inspired by the image content  
- 🎯 Use case: Creative writing aid, idea prompts, accessibility applications

---

## 🧱 Architecture

[Image] ──► ResNet Encoder ──► Embedding Vector ──► GPT-2 ──► Narrative Output


- `ResNet`: Extracts high-level features from the image  
- `GPT-2`: Takes those features as seed input and generates an open-ended story  

We also explore custom Transformer decoder variants, caption-first approaches, and prompt-tuned GPT-2 responses.

---

## 🧪 Dataset

- 🖼️ **Flickr8k**  
  - 8,000 images with 5 captions each  
  - Used to align visual features with natural language

---

## 💡 Sample Output

**Input Image:**  
![sample](./samples/caption_sample.jpg)

**Generated Story:**  
> "A young boy runs along the beach, waves crashing beside him as the sun begins to set. It’s his first evening by the sea, and the salty air fills him with joy. In his small hands, he clutches a shell he found moments ago — a treasure in a land of endless water."

---

## 🧰 Tech Stack

- Python, TensorFlow, HuggingFace Transformers
- ResNet (image encoder)
- GPT-2 (pretrained text generation)
- Flickr8k dataset
- Matplotlib (visualization)

---

## 📦 Setup

```bash
pip install -r requirements.txt
python main.py  # or run the notebook

