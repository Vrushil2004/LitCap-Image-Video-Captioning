
# LiteCap — Deep Image Captioning (BLIP)

This project is a ready-to-run **Streamlit** app that generates **deep captions** for any image using the pretrained **BLIP** model from Hugging Face.

## ✨ Features
- **Deep captions** via `Salesforce/blip-image-captioning-base`
- Works on **CPU or GPU** (auto-detects `cuda` if available)
- Adjustable generation settings (beam search, max tokens, etc.)

## 🚀 Quickstart

```bash
# 1) (Recommended) Create a virtual environment
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate

# 2) Install dependencies
pip install -r requirements.txt

# 3) Run the app
streamlit run app.py
```

Then open the URL shown in the terminal (usually http://localhost:8501).

> On the **first run**, the BLIP model is downloaded from Hugging Face. Make sure you have **internet** the first time.
> After that, the model is cached locally and reused.

## 🧠 Model
- `Salesforce/blip-image-captioning-base` via `transformers`

## 🖼️ Usage
1. Click **Upload an image** (JPG/PNG/WEBP).  
2. The app shows the image and generates a caption.  
3. Optionally tweak **Advanced settings** for different caption styles.

## 🧪 Tips
- CPU works fine for demos; a **GPU** will speed up generation.  
- If you face `torch` install issues on some systems, see: https://pytorch.org/get-started/locally/

## 📦 Make it a GitHub repo
```bash
git init
git add .
git commit -m "feat: BLIP image captioning app"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## 📄 License
MIT
