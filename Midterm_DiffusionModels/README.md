# Midterm — Creating Images with Diffusion Models

This midterm project explores the development, training, and evaluation of a **conditional diffusion model** using the MNIST dataset. The work includes a written technical report and a Jupyter Notebook demonstrating forward diffusion, reverse denoising, U-Net implementation, class conditioning, and CLIP-based evaluation.

## 📄 Included Files
- **MD_Report_Ruben_Valenzuela_ITAI.pdf** — Full written midterm report  
- **MD_Notebook_Ruben_ITAI.ipynb** — Complete implementation notebook  
- **MD_Notebook_Ruben_ITAI.pdf** — PDF export of the notebook  

## 🧠 Key Topics Covered
- Forward & reverse diffusion processes  
- Gaussian noise scheduling  
- Conditional U-Net architecture  
- Time-step embeddings  
- Noise prediction with MSE loss  
- CLIP-based semantic evaluation  
- Visual analysis of generated samples  

## 🏗️ Model Architecture
The diffusion model uses a **U-Net** with:
- Encoder–decoder symmetry  
- Skip connections for detail preservation  
- Time embeddings to represent noise level  
- Optional digit-class conditioning  

This allows the model to gradually reconstruct digits from pure noise.

## 📉 Training Observations
Results improved consistently across epochs:
- Early stages: blurry or noisy images  
- Later stages: digits become clear and well defined  

Time-step embeddings were critical to letting the model understand *where in the denoising schedule* it was.

## 🧪 CLIP-Based Evaluation
CLIP was used to evaluate semantic similarity between generated digits and prompts like:

- “a handwritten 3”
- “a blurry number”
- “a handwritten 0”

Digits with simple geometry performed best (0, 1, 7), while others (5, 8, 9) were more difficult.

## 🌍 Applications
Diffusion models are widely used for:
- Data augmentation  
- Image restoration  
- AI image generation  
- Educational demonstrations of generative modeling  

## 🚀 Future Improvements
Suggested enhancements include:
- Adding attention layers  
- Using EMA weights  
- Training longer for better clarity  
- Implementing classifier-free guidance  

## ✨ Reflection
This midterm provided a practical understanding of how diffusion models generate structured images from noise, and how CLIP can be used to evaluate their semantic quality.

---

### 🔗 Author
**Ruben Valenzuela** — ITAI 2376  
