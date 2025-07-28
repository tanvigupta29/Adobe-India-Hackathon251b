# Adobe-India-Hackathon251b
# 📄 Intelligent PDF Heading Detection – Interactive Web App

This project provides a **user-friendly interface** for extracting structured outlines from PDF documents using a trained machine learning model. It detects headings (Title, H1, H2, H3) in PDFs and outputs a hierarchical structure in real time.

🔗 GitHub Repository: [Adobe-India-Hackathon25](https://github.com/tanvigupta29/Adobe-India-Hackathon25)

---

## 💡 Overview

Navigating unstructured PDFs is hard — especially when there's no embedded Table of Contents. This app uses a **machine learning model trained on font and layout features** to detect heading levels from text lines, then presents them as an **expandable, clickable outline.**

Built as a lightweight frontend-backend tool, the system enables:
- Easy PDF upload
- Automatic heading detection
- Hierarchical outline rendering
- Real-time preview of content sections

---

## 🧭 Key Features

✅ Upload any standard text-based PDF  
✅ Automatic detection of `Title`, `H1`, `H2`, and `H3` headings  
✅ Real-time visualization of the document’s structure  
✅ Expand/collapse outline view  
✅ Display page content by clicking on a heading  

---

## 🧠 ML Approach Behind the Scenes

1. **PDF Parsing**  
   Extracts each line’s text, font size, bold/italic status, position using `PyMuPDF`.

2. **Feature Engineering**  
   Generates features like:
   - Font size (normalized)
   - Capitalization ratio
   - Is bold or italic?
   - Line length
   - Y-position on page

3. **Classification**  
   Pre-trained `Random Forest` model classifies each line into:
   - `Title`
   - `H1`, `H2`, `H3`
   - or `None` (not a heading)

4. **Structured Output**  
   A hierarchy is built based on predictions, which feeds into the UI as a nested structure.

---

## 🧰 Technologies Used

| Component        | Tech Used                            |
|------------------|--------------------------------------|
| Frontend         | HTML, CSS, JavaScript (Vanilla)      |
| Backend API      | Python + Flask                       |
| PDF Parsing      | PyMuPDF (`fitz`)                     |
| ML Inference     | scikit-learn (`joblib` model loading)|
| UI Rendering     | DOM manipulation with JS             |

---

## 🛠️ How to Build and Run Locally

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/tanvigupta29/Adobe-India-Hackathon25.git
cd Adobe-India-Hackathon25

