# Dense-PMSFNet: Retinal Vasculature and FAZ Segmentation in OCTA Images
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-brightgreen.svg)]()
This repository provides a clean and independent implementation of **Dense-PMSFNet**, a DenseNet-based pyramidal multi-scale fusion network for accurate segmentation of retinal microvasculature (arteries, veins, capillaries) and the Foveal Avascular Zone (FAZ) in OCTA images.

Originally published in:  
**IEEE LATIN AMERICA TRANSACTIONS, Apr 2025**

---

## 📁 Repository Structure

- `data_loader.py` – Preprocess OCTA images and save them as compressed `.npz`
- `train.py` – Trains the Dense-PMSFNet model using configs and dataset
- `test.py` – Evaluates the model and generates test predictions
- `config.yaml` – Configuration file for training/testing
- `requirements.txt` – Python dependencies
- `models/` – Directory with supporting models used for comparison
- `model.py` – Core implementation of Dense-PMSFNet

---

## 🚀 Getting Started

### ✅ Clone the Repository
```bash
git clone https://github.com/nisan-ai/Dense-PMSFNet-OCTA.git
cd Dense-PMSFNet-OCTA

```

### ✅ Create a Virtual Environment & Install Dependencies
```bash
python -m venv env
# Activate environment
# Windows:
env\Scripts\activate
# Linux/Mac:
source env/bin/activate

pip install -r requirements.txt
```

---

## 🧪 Dataset Preparation

Preprocess and save dataset to `dataset.npz`:
```bash
python data_loader.py --config config.yaml
```

---

## 🧠 Training

Train the Dense-PMSFNet model:
```bash
python train.py --config config.yaml
```

---

## 📊 Testing & Evaluation

Run the test script on the saved model:
```bash
python test.py --config config.yaml
```

---

## 📄 Citation

If you use this work in your research, please cite the original paper:

```bibtex
@ARTICLE{10930374,
  author={Raja, Nisan Pranavah and Sarvesan, Srivatsan and Thomas, Anju and P Gopi, Varun},
  journal={IEEE Latin America Transactions}, 
  title={Dense-PMSFNet: DenseNet Pyramidal Multi-Scale Fusion Network for Retinal Vasculature and FAZ Segmentation in OCTA Images}, 
  year={2025},
  volume={23},
  number={4},
  pages={312-322},
  keywords={Image segmentation;Retina;Feature extraction;Accuracy;Veins;Arteries;Decoding;Deep learning;Convolution;Robustness;Optical Coherence Tomography Angiography, Artificial Intelligence, vein, artery, capillary, FAZ, densenet encoder, multiscale pyramidal fusion module (MSPFM), deep fusion, deep learning.},
  doi={10.1109/TLA.2025.10930374}
}
```

---

## 👤 Maintainer

This repository is maintained by Nisan Pranavah Raja, the first author and lead contributor of the original IEEE publication. While the research and model development were carried out collaboratively with co-authors, this GitHub implementation has been independently refined, documented, and curated by Nisan to enable broader accessibility, reproducibility, and real-world application..

🔗 [Google Scholar](https://scholar.google.com/citations?user=_PW0aeYAAAAJ&hl=en)  
🔗 [LinkedIn](https://www.linkedin.com/in/nisan-pranavah-raja)  

