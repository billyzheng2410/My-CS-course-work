This notebook (`a1.ipynb`) demonstrates three stages of regression/classification training:

1. **Linear Regression**  
   - Implemented in closed form (normal equation).  
   - Implemented with **full-batch gradient descent** as a baseline.  
   - Evaluated on the Parkinson’s Telemonitoring dataset (`motor_UPDRS` target).

2. **Logistic Regression (Full Batch)**  
   - Implemented with gradient descent using the entire dataset at each step.  
   - Evaluated on the WDBC Breast Cancer dataset (`Diagnosis` mapped M=1, B=0).

3. **Mini-batch Stochastic Gradient Descent (SGD)**  
   - A reusable optimizer class (`MiniBatchOptimizer`) is defined.  
   - Applied to both Linear and Logistic Regression.  
   - Supports cost history recording, early stopping, and evaluation curves.

---

## Requirements

- Python 3.9+
- Dependencies are listed in `requirements.txt`

Install them:

```bash
pip install -r requirements.txt
```

---

## How to Run

### Option A: Google Colab

1. Upload `a1.ipynb`, `requirements.txt`, and `README.md` to your Drive or open the notebook directly in Colab.
2. (Optional) Change runtime to CPU (GPU not needed).
3. Click **Runtime ▸ Run all**.

### Option B: Local Python Environment

1. Clone or download the project folder containing `a1.ipynb`, `requirements.txt`, and `README.md`.
2. Create and activate a virtual environment (recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # Linux / macOS
   venv\Scripts\activate      # Windows
   ```
3. Install dependencies from `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook or JupyterLab:

   ```bash
   jupyter notebook a1.ipynb
   # or
   jupyter lab a1.ipynb
   ```
5. Run all cells in order (**Cell ▸ Run All**).

The notebook will:

- Download the UCI datasets
- Clean and preprocess features (drop IDs, encode categorical, standardize)
- Run **Linear Regression** (closed form & full-batch GD)
- Run **Logistic Regression** (full-batch GD)
- Run **Mini-batch SGD** on both tasks
- Plot training/learning curves and report metrics

---

**Note:** Task 3.3 for logistic regression takes a long time to run. Please wait a few seconds!

---

## Output / What to Expect

- How the data is processed
- Logistic Regression: Accuracy, learning curves
- Mini-batch SGD: Cost histories, comparisons to full-batch, test performance
- The plots show how training behaves under different optimization methods
- Experiments beyond tasks

---

