# MiniTweetGPT-A-small-GPT-like-model-for-tweets-
MiniTweetGPT – A lightweight GPT-like language model trained on ChatGPT-related tweets using PyTorch and Transformers. It can generate tweet-style text and learn patterns from social media language.
🔹 Features

✅ Small-scale transformer-based model
✅ Trained on a real-world Twitter dataset
✅ Uses PyTorch & Hugging Face Transformers
✅ Tokenization with BERT-based tokenizer
✅ Fine-tunable for better results
📥 Setup Kaggle API for Dataset Download
1️⃣ Get Your Kaggle API Key

    Go to Kaggle and log in.
    Click your profile picture → "Account".
    Scroll to the API section and click "Create New API Token".
    A file named kaggle.json will be downloaded.

2️⃣ Upload kaggle.json to Google Colab

from google.colab import files

# Upload kaggle.json
files.upload()

3️⃣ Move API Key to Correct Location

import os
import shutil

# Create Kaggle directory
os.makedirs("/root/.kaggle", exist_ok=True)

# Move API key
shutil.move("kaggle.json", "/root/.kaggle/")
os.chmod("/root/.kaggle/kaggle.json", 600)

4️⃣ Install Kaggle & Download Dataset

!pip install kaggle
!kaggle datasets download tariqsays/chatgpt-twitter-dataset --unzip -p /content/data

🚀 Next Steps

🔹 Train the model further for better tweet generation
🔹 Fine-tune using pre-trained GPT models (e.g., GPT-2)
🔹 Improve text coherence & creativity
