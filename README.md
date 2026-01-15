# 🚶‍♂️ Person Re-Identification (ReID) — AML Course Project

Advanced Machine Learning (AML) course project (Sapienza University of Rome).  
This repository explores **Person Re-Identification**: recognizing the same individual across different cameras, viewpoints and conditions (core component of modern surveillance and multi camera analytics).

📄 **Report (PDF):** `report/main.pdf`

---

## 📌 What’s inside

The project studies and experiments with multiple ReID approaches, including:
- **Metric learning** objectives (e.g. contrastive / triplet-style training)
- **Pretraining** effects on large scale human datasets (e.g. **LUPerson**)
- Architectures and training pipelines built from scratch and evaluated on standard benchmarks

Evaluation is performed on common ReID datasets (notably **Market-1501** and **CUHK-03**) using:
- **Rank-1 accuracy**
- **mAP (mean Average Precision)**

(Full details, experimental settings and results are in the report.)

---

## 📂 Repository structure

- `report/` — LaTeX sources + compiled PDF
  - `report/main.pdf` — final report
  - `report/sections/` — report sections
  - `report/img/` — figures used in the report
- `*.ipynb` — experiment notebooks:
  - `Contrastive.ipynb`
  - `ViTvae.ipynb`
  - `LA_Transformers.ipynb`
  - `LUPerson_pretraining.ipynb`
  - `Dataset_Convert.ipynb`
  - `testing.ipynb`

---

## ▶️ How to use

This project is primarily notebook driven.

### 1) Environment
Create a fresh environment (conda or venv) and install the required packages used in the notebooks.  
Since course projects often evolve quickly, the simplest approach is:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -U pip
# then install the packages referenced in the notebooks (torch, torchvision, numpy, etc.)
```

If you already have a working ML environment you can directly open the notebooks and run them there.

### 2) Notebooks
Open Jupyter and run the notebooks in the repository root:

```bash
jupyter lab
```

Recommended starting point:
- **`testing.ipynb`** (if you want a quick overview / sanity checks)
- then the specific experiment notebook of interest (contrastive, transformer-based, VAE, pretraining)

---

## 📄 Report

The write up includes:
- problem definition and background
- methodology (models, losses, pretraining)
- experimental setup and datasets
- results and discussion
- conclusions and limitations

➡️ **`report/main.pdf`**

---

## ⚠️ Notes / scope

- This is a **course project**, not a production library.
- Code is organized for experimentation and clarity rather than packaging.
- Results should be interpreted in the context of the described setup and compute constraints.

---

## 👥 Authors

- **Paolo Cursi** (2155622)  
- **Stefano Saravalle** (1948684)  
- **Michele Palma** (1849661)  
- **Pietro Signorino** (2149741)

Sapienza University of Rome

---

## 📝 License

Released for **educational and academic purposes**.
