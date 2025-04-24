# 👗 Fashion AI Recommendation System

An AI-powered content-based fashion recommendation system that suggests visually similar outfits using image embeddings. This project combines the power of OpenCLIP, ChromaDB, and computer vision to enhance the fashion discovery experience.

## 📌 Overview

This system allows users to upload or select a fashion image and receive visually similar outfit recommendations. By leveraging deep learning models and a vector database, it mimics how humans visually recognize similar clothing styles.

## 📚 Dataset

- **Dataset Name:** [Fashionpedia](https://huggingface.co/datasets/detection-datasets/fashionpedia)  
- **Source:** Hugging Face  
- The dataset includes 48,000+ clothing items across multiple categories with bounding boxes and detailed annotations. It is ideal for building image-based retrieval systems in the fashion domain.

## 🧠 Tech Stack

- **Language:** Python  
- **Libraries & Tools:** 
  - OpenCLIP (for image feature extraction)  
  - ChromaDB (for storing and querying vector embeddings)  
  - NumPy, PIL (for preprocessing)  
  - Google Gemini (optional: for LLM-powered recommendation layer)

## 🌟 Key Features

- 🔍 **Visual Similarity Search:** Upload a clothing image and get outfit suggestions based on visual features.
- 🧠 **Feature Extraction:** Utilizes OpenCLIP to generate meaningful embeddings from fashion images.
- 🗂️ **Vector Search:** ChromaDB enables efficient similarity search using cosine or dot product metrics.
- 🧰 **Image Preprocessing:** Custom loader to resize and clean images for consistent embedding quality.
- 🎯 **Scalable Retrieval:** Supports large-scale fashion image datasets with high performance.

## 📁 Project Structure

```
fashion-ai-recommendation/
│
├── data/                  # Contains sample fashion images
├── embeddings/            # Precomputed or generated image vectors
├── utils/                 # Scripts for loading images, generating embeddings
├── fashionpedia_loader.py # Custom loader for Hugging Face Fashionpedia dataset
├── app.py                 # Main script for recommendation logic
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
```

## ⚙️ How to Run

1. **Clone the Repository**
```bash
git clone https://github.com/Mahalakshmi-P28/fashion-ai-recommendation.git
cd fashion-ai-recommendation
```

2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

3. **Download the Dataset**  
Use Hugging Face's `datasets` library or download it manually:
```bash
pip install datasets
```

```python
from datasets import load_dataset
dataset = load_dataset("detection-datasets/fashionpedia")
```

4. **Run the App**
```bash
python app.py
```

## 💡 Applications

- Fashion E-commerce  
- Smart Wardrobe Suggestions  
- Visual Search Systems  
- AI-Powered Styling Assistants

## 📬 Contact

For queries or collaborations, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/pilla-mahalakshmi-09642a259/) or open an issue in this repository.
