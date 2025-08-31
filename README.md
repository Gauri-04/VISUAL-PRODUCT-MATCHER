🔍 Visual Product Matcher  

A sleek, responsive web app that helps you **find visually similar products** by simply uploading an image.  
Powered by **TensorFlow.js (MobileNet)**, it runs entirely in your browser — ⚡ fast, private, and no backend required!  

---

✨ Features
- 📤 Upload an image or paste a URL  
- 👀 Live image preview before searching  
- 🧠 AI-powered similarity search with MobileNet embeddings  
- 🎚 Adjustable similarity threshold  
- 🗂 Filter by category & sort by score  
- 📱 Fully responsive (mobile + desktop)  
- 🎨 Clean, modern UI  

---

🚀 Live Demo
Deployed with **Vercel** 👉 [Visual Product Matcher](https://vercel.com/gauri-guptas-projects/visual-product-matcher)  

---

📂 Dataset
- Demo uses **placeholder product images** (`picsum.photos`).  
- Swap in your own catalog via a `products.json` file for realistic results.  

---

🛠 Tech Stack
- **Frontend**: HTML, CSS, JavaScript  
- **AI Model**: TensorFlow.js (MobileNet)  
- **Deployment**: Vercel  

---

📖 Approach
This app extracts **image embeddings** using MobileNet directly in the browser.  
Uploaded images are compared to pre-computed product embeddings using **cosine similarity**, then filtered & sorted based on user settings.  

The focus was on **simplicity and usability**: responsive UI, error handling, clean design, and zero backend dependencies. Deployment was done via **Vercel**, ensuring instant access and auto-updates from GitHub.  

---
💡 *Tip: Replace the demo dataset with your own products to turn this into a real e-commerce visual search tool!*  
