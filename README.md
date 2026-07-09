# 🖼️ Multilingual Image Caption Generator

An AI-powered **Multilingual Image Caption Generator** that automatically generates descriptive captions for images in **English**, translates them into **Hindi** and **Marathi**, and converts the generated captions into speech using **Google Text-to-Speech (gTTS)**.

The project combines **Computer Vision**, **Deep Learning**, **Natural Language Processing (NLP)**, **Machine Translation**, and **Speech Synthesis** to make image understanding more accessible across multiple languages.

---

## 📖 Project Overview

Image captioning is an important application of Artificial Intelligence that combines Computer Vision and Natural Language Processing. This project uses a Deep Learning-based encoder-decoder architecture with an attention mechanism to generate meaningful captions for images.

The generated English caption is translated into Hindi and Marathi using **Meta AI's NLLB-200 multilingual translation model**. Finally, the translated captions are converted into speech using **Google Text-to-Speech (gTTS)**.

The model is trained on the **Flickr8k Dataset** and evaluated using the **BLEU Score** metric.

---

# ✨ Features

- 🖼️ Automatic Image Caption Generation
- 🌍 Caption Translation
  - English
  - Hindi
  - Marathi
- 🔊 Text-to-Speech Generation
- 🤖 Attention-based Image Captioning
- 📚 Beam Search Caption Decoding
- 💾 Model Training & Saving
- 📊 BLEU Score Evaluation
- 📈 Performance Analysis & Visualization
- 📤 Upload Custom Images for Caption Generation

---

# 🛠️ Tech Stack

### Programming Language
- Python

### Deep Learning
- PyTorch
- TorchVision

### Computer Vision
- EfficientNet-B0

### NLP & Translation
- Hugging Face Transformers
- Meta NLLB-200 Distilled 600M

### Text-to-Speech
- Google Text-to-Speech (gTTS)

### Dataset
- Flickr8k Dataset

### Python Libraries
- NumPy
- Pandas
- Pillow
- Matplotlib
- NLTK
- Transformers
- gTTS

---

# 🧠 Model Architecture

```
                Input Image
                     │
                     ▼
          Image Preprocessing
                     │
                     ▼
          EfficientNet-B0 Encoder
                     │
                     ▼
        Attention-based LSTM Decoder
                     │
                     ▼
          English Caption Generation
             │                 │
             ▼                 ▼
     Hindi Translation    Marathi Translation
             │                 │
             └─────────┬────────┘
                       ▼
          Google Text-to-Speech (gTTS)
                       │
                       ▼
        Text + Audio Output (3 Languages)
```

---


---

# ⚙️ Working

### Model Training

The training pipeline performs the following tasks:

- Dataset preprocessing
- Caption cleaning
- Vocabulary creation
- EfficientNet feature extraction
- Attention-based LSTM training
- Beam Search implementation
- Model evaluation
- Model saving

---

### Caption Generation

The inference pipeline performs the following tasks:

- Load the trained model
- Upload an image
- Generate an English caption
- Translate the caption into Hindi
- Translate the caption into Marathi
- Generate speech in all three languages
- Display captions and audio output

---

# 📊 Model Evaluation

The model was evaluated using the **BLEU Score**, a widely used evaluation metric for image caption generation.

| Metric | Value |
|---------|-------|
| BLEU Score | **0.21** |

Additional analysis performed:

- Caption Length Distribution
- Ground Truth vs Predicted Caption Length
- Inference Time Analysis
- Word Frequency Analysis
- Multilingual Caption Comparison

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/ChaitaliWaware74/Image_Caption_Generator.git
```

Go to the project directory

```bash
cd Image_Caption_Generator
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Training

Run

```bash
python train_model.py
```

This script:

- Loads the Flickr8k dataset
- Trains the image captioning model
- Evaluates the model
- Saves the trained model

---

# ▶️ Generate Captions

Run

```bash
python generate_caption.py
```

This script allows users to:

- Upload any image
- Generate captions
- Translate captions
- Generate audio in English, Hindi, and Marathi

---

# 📸 Screenshots

## Upload Image

<img width="922" height="592" alt="image" src="https://github.com/user-attachments/assets/80b798c5-e534-4160-bc0b-fb0b3758d840" />


---

## English, Hindi and Marathi Caption

<img width="855" height="432" alt="image" src="https://github.com/user-attachments/assets/75d65349-65df-49dc-a215-484ee1c3face" />



---

## Audio Generation

<img width="912" height="602" alt="image" src="https://github.com/user-attachments/assets/d734ab2a-d0bd-4647-a9c7-0bbe4caa3426" />

---

# 📄 Trained Model

The trained model (`image_caption_model.pth`) is **not included** in this repository because it exceeds GitHub's file size limit.

To run the project:

- Train the model using `train_model.py`, or
- Place the trained model inside the project directory before running `generate_caption.py`.

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Computer Vision
- Deep Learning
- Image Captioning
- Natural Language Processing
- Machine Translation
- Attention Mechanism
- Beam Search Decoding
- Transfer Learning
- PyTorch
- Hugging Face Transformers
- Google Text-to-Speech

---

# 🔮 Future Enhancements

- Support additional Indian languages
- Improve caption accuracy using Transformer-based decoders
- Web deployment using Streamlit
- Real-time caption generation
- Voice input support
- Larger datasets for improved generalization

---

# 👩‍💻 Author

**Chaitali Waware**

Computer Engineering Student

### Interests

- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Deep Learning
- Data Analytics
