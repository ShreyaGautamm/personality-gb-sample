# Personality Shapes Gender Bias in Persona-Conditioned LLM Narratives
### Interactive Research Showcase & Demo Website

This repository contains the interactive research demonstration website for the paper:

> **Personality Shapes Gender Bias in Persona-Conditioned LLM Narratives Across English and Hindi: An Empirical Investigation**  
> *Tanay Kumar\*, Shreya Gautam\*, Aman Chadha†, Vinija Jain†, Francesco Pierri*  
> Politecnico di Milano, Apple, Meta  
> **arXiv:2604.23600v2 [cs.CL]**

---

## 🌟 Interactive Features Included

1. **Qualitative Story Comparator**:
   - Side-by-side Male vs. Female persona narratives under identical personality conditioning.
   - Color-coded text segment annotations (Overt authority defiance, covert domestic sabotage, grandiosity vs. emotional vulnerability).
   - Sentence-level IndicSBERT difference-of-cosines bias scores.
   - Includes English and Hindi stories with English translations.

2. **IndicSBERT Centroid Metric Explorer**:
   - Interactive difference-of-cosines spectrum slider (`[-1.0, +1.0]`).
   - Clickable presets demonstrating how phrases and grammatical inflections lean stereotypic.

3. **Empirical Regression & Model Benchmark Visualizer**:
   - OLS regression effect forest plot showing how Dark Triad traits (Machiavellianism, Psychopathy) systematically amplify male-stereotypic framing.
   - Benchmark breakdown across 6 model architectures (GPT-5 nano, LLaMA-3.3, DeepSeek-R1, Gemma-3, Falcon-Mamba, Mixtral) in English and Hindi.

4. **Human Validation Mini-Quiz**:
   - Interactive blind comparison game based on the 100-pair human annotation experiment (Fleiss' $\kappa = 0.66\text{--}0.69$).

5. **50 Occupations Explorer**:
   - Filterable and searchable table of 25 male-stereotyped and 25 female-stereotyped occupations, contextual artifacts, and task scenarios grounded in the Indian socio-cultural setting.

6. **BibTeX Citation Card**:
   - One-click copy with instant feedback.

---

## 🚀 How to Preview Locally

No Node.js or build tools required! You can preview it immediately:

### Method 1: Using Python (Recommended)
Open your terminal in this directory and run:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000` in your web browser.

### Method 2: Direct File Open
You can also directly double-click `index.html` to open it in Chrome, Safari, or Firefox.

---

## 🌐 How to Deploy to Netlify (Free Hosting)

You can host this website on Netlify for free in just a couple of minutes using either of these two methods:

### Option A: Via GitHub (Recommended for Continuous Updates)
1. Initialize git and push this folder to your GitHub account:
   ```bash
   git init
   git add .
   git commit -m "Initial research website commit"
   git branch -M main
   # Add your remote repository:
   # git remote add origin https://github.com/<your-username>/personality-gender-bias.git
   # git push -u origin main
   ```
2. Go to [Netlify](https://app.netlify.com/) and sign in.
3. Click **"Add new site"** → **"Import an existing project from Git"** → choose **GitHub**.
4. Select your `personality-gender-bias` repository.
5. In the build settings:
   - **Build command**: *(leave blank)*
   - **Publish directory**: `.` (or leave as root)
6. Click **"Deploy site"**. Netlify will give you a live URL (e.g., `https://personality-gender-bias.netlify.app`), and any future Git push will auto-deploy updates!

### Option B: Netlify Drag & Drop (Instant - No Git Required)
1. Go to [Netlify Drop](https://app.netlify.com/drop).
2. Drag and drop this whole `personality-gender-bias` folder into the browser window.
3. Your site will be live immediately with a free HTTPS URL!

---

## 📁 Repository Structure

```
personality-gender-bias/
├── index.html        # Main landing page and interactive interface
├── netlify.toml      # Netlify deployment and header configuration
├── README.md         # Instructions and documentation
├── css/
│   └── styles.css    # Clean academic styling, dark-mode gradients & responsive layout
└── js/
    ├── data.js       # Complete research dataset (narratives, stats, occupations, quiz)
    └── app.js        # Interactive UI logic, slider, comparator, quiz & table
```

---

## 📖 Citation

```bibtex
@article{kumar2026personality,
  title={Personality Shapes Gender Bias in Persona-Conditioned LLM Narratives Across English and Hindi: An Empirical Investigation},
  author={Kumar, Tanay and Gautam, Shreya and Chadha, Aman and Jain, Vinija and Pierri, Francesco},
  journal={arXiv preprint arXiv:2604.23600},
  year={2026}
}
```
