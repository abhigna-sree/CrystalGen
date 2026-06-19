# 🧊 CrystalGen: AI-Powered Crystal Structure Generator

CrystalGen is an AI-powered web application that generates and visualizes crystal structures using a Conditional Variational Autoencoder (CVAE). The platform enables users to configure parameters such as space group, chemical composition, number of atoms, and temperature to generate realistic 3D crystal lattices in real time.

---

## 🌐 Overview

CrystalGen combines modern deep learning techniques with materials science tools to simplify crystal structure generation and visualization.

### Key Technologies

- 🧠 Conditional Variational Autoencoder (CVAE) for crystal generation
- 🔬 Pymatgen for CIF parsing and structure validation
- 🧱 PyTorch Geometric (PyG) for graph-based crystal representation
- 🌍 Flask backend with HTML/CSS/JavaScript frontend
- 🎨 Interactive 3D visualization using Plotly, Three.js, and Py3Dmol

---

## ✨ Features

- Generate crystal structures from user-defined parameters
- Interactive 3D visualization of generated lattices
- CIF file preview and download support
- Model performance dashboard with training metrics
- Graph-based crystal representation for improved learning
- Fast and accurate structure generation using deep learning

---

## 📁 Project Structure
<img width="266" height="717" alt="510673558-c61a8c5f-e502-4925-bd18-b0011ce574d3" src="https://github.com/user-attachments/assets/885cfcf0-7ada-4352-ae91-da0a50157aa5" />

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/abhigna-sree/CrystalGen.git
cd CrystalGenProject-master
```

### 2. Install Python Dependencies

```bash
pip install flask flask-cors flask-bcrypt pyjwt pymongo ase pymatgen torch torch-geometric
```

### 3. Install Visualization Dependencies

```bash
npm install 3dmol
```

### 4. Run the Application

```bash
cd model
python app.py
```

The application will start on:

```text
http://localhost:5000
```

---

## 🧠 Model Architecture

CrystalGen uses a Conditional Variational Autoencoder (CVAE) to learn crystal formation patterns and generate valid crystal structures.

### Architecture Overview

#### Encoder
- Converts crystal graphs into compact latent representations
- Extracts structural and compositional features

#### Latent Diffusion Layer
- Introduces controlled stochastic variations
- Improves diversity of generated structures

#### Decoder
- Reconstructs crystal structures from latent vectors
- Predicts atomic coordinates and lattice parameters

#### Output
- Generated crystal structure
- CIF file generation
- Interactive 3D visualization

---

## 📈 Model Performance

| Metric | Old Model | New Model |
|----------|----------|----------|
| Parameters | 2.47M | 18.07M |
| Average Loss | 54.8 | 12.3 |
| Accuracy | 72% | 91% |
| Quality | Moderate | Excellent |

### Improvements

- ✅ Better crystal reconstruction accuracy
- ✅ Lower reconstruction loss
- ✅ Stable model training
- ✅ Faster inference
- ✅ Higher-quality generated structures

---

## 💻 Web Interface

### 🏠 Home Page

Users can configure:

- Space Group (1–230)
- Chemical Composition (e.g., FeO, SiO₂)
- Number of Atoms
- Temperature

Click **Generate Structure** to create a new crystal lattice.

---

### 📊 Results Page

Displays:

- Interactive 3D crystal visualization
- Generated CIF file preview
- Downloadable structure file
- Crystal information summary

---

### 📈 Metrics Dashboard

View:

- Training and validation losses
- Model comparison statistics
- Performance charts
- Accuracy metrics

---

## 🔍 API Routes

| Route | Method | Description |
|---------|---------|---------|
| `/` | GET | Main application interface |
| `/generate` | POST | Generate a crystal structure |
| `/results` | GET | Display generated structure and CIF |

---

## 📊 Training Workflow

### Step 1: Data Preparation
- Load CIF files
- Parse structures using Pymatgen

### Step 2: Graph Construction
- Convert crystal structures into graph representations using PyTorch Geometric

### Step 3: Model Training
- Train CVAE using:
  - Reconstruction Loss
  - KL Divergence Loss

### Step 4: Evaluation
- Validate generated structures
- Monitor accuracy and loss metrics

### Step 5: Structure Generation
- Generate novel crystal structures
- Visualize outputs interactively

---

## 📉 Example Results

| Metric | Old Model | New Model |
|----------|----------|----------|
| Reconstruction Loss | 0.125 | 0.034 |
| KL Divergence | 0.015 | 0.006 |
| Generation Accuracy | 72% | 91% |
| Inference Time | 0.42s | 0.18s |

---

## 🧩 Generation Pipeline

```text
CIF Dataset
      ↓
Pymatgen Parser
      ↓
Crystal Graph Builder (PyG)
      ↓
CVAE Encoder
      ↓
Latent Space Diffusion
      ↓
CVAE Decoder
      ↓
Crystal Structure Generation
      ↓
CIF Export
      ↓
3D Visualization
      ↓
Web Interface
```

---

## 🚀 Future Enhancements

- Support for multi-component crystal systems
- Property prediction integration
- Materials database connectivity
- Crystal stability estimation
- Advanced diffusion-based generation models
- Cloud deployment support

---

## ⭐ Conclusion

CrystalGen bridges the gap between artificial intelligence and materials science by providing an intuitive platform for crystal structure generation, visualization, and exploration. By leveraging graph neural networks and CVAE-based generative modeling, the system delivers fast, accurate, and visually interactive crystal generation workflows.
