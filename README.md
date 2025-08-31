# Visual Product Matcher

A lightweight web application that finds visually similar products based on an uploaded image.  
Built using **HTML, CSS, JavaScript, and TensorFlow.js (MobileNet)**, the app runs entirely in the browser — no backend required.  

## Features
- Upload image (file) or paste image URL  
- Live preview of query image  
- Finds similar products from a dataset using cosine similarity on image embeddings  
- Filters: similarity threshold, category filter, sorting options  
- Responsive, mobile-friendly UI with light/dark mode toggle  
- Simple deployment on GitHub Pages / Netlify / Vercel  

## Demo Dataset
The included dataset uses 50 placeholder product images (`picsum.photos`). Replace with your own product catalog for real-world usage.

## Deployment
1. Push this repo to GitHub.  
2. Enable GitHub Pages (Settings → Pages → Branch: `main`).  
   - Your app will be live at `https://<username>.github.io/visual-product-matcher/`.  
3. Alternatively, deploy directly on [Netlify](https://www.netlify.com) or [Vercel](https://vercel.com).  

## Approach (≤200 words)
The goal was to create a responsive, production-quality demo with minimal setup. I chose **TensorFlow.js MobileNet embeddings** to compute feature vectors directly in the browser, avoiding the need for a backend or API. A small product dataset (50+ images with metadata) is stored locally in the code. When a user uploads or links an image, the model generates an embedding. Cosine similarity is then computed between the query embedding and pre-computed product embeddings to find matches. Results are filtered by similarity threshold, category, and sorting preferences.  

The UI is built with plain **HTML/CSS/JS**, optimized for responsiveness, with skeleton loading states, error handling, and a dark/light mode toggle for better UX. Deployment is simplified to a static HTML file, making it portable and easy to host on GitHub Pages or any free hosting service.  
