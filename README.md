# AI-Layoff-Risk-Predictor
![AI101 Mini-Project](https://img.shields.io/badge/AI101%20Mini--Project-green)
![Team 28](https://img.shields.io/badge/Team-28-green)
![Python 3.12+](https://img.shields.io/badge/Python-3.10%2B-green?logo=python&logoColor=white)

Predicts an employee’s layoff risk (Low, Medium or High) from job and AI-use data
## Team and roles

| Member | Entry no. | Role | 
|---|---|---|
| Shreyas Iyer | 2026EEB1412 | Documentation lead |
| Hisham | 2026MCB1530 | Execution lead |
| Saniya Jain | 2026DAB1306 | PPT lead |
| Bhakti Bagade | 2026AIB1027 | Video lead |

## Setup

Python 3.12 or newer. The notebook was last run on Python 3.14.6, and its code was re-checked on Python 3.12 with the versions in `requirements.txt` (same final metrics).

```bash
git clone https://github.com/Shreyas-IITRPR/AI-Layoff-Risk-Predictor.git
cd AI-Layoff-Risk-Predictor
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
```
## How to run

1. From the repo folder, run `jupyter notebook`.
2. Open `ai101_team28.ipynb`.
3. Choose **Kernel → Restart & Run All**. It finishes in well under a minute and saves the plots and `metrics.json` in `outputs/` (and `training_curve_gd.png` in the repo folder).

The data path is relative (`ai-impact-jobs-layoff-risk-dataset.csv`), so the notebook and the CSV must stay in the same folder.

## Expected output

| | Train | Test |
|---|---|---|
| Accuracy | 0.941000 | 0.937750 |
| Precision (macro) | 0.940924 | 0.937548 |
| Recall (macro) | 0.940860 | 0.937530 |
| F1 (macro) | 0.940888 | 0.937535 |
| ROC AUC (macro, one-vs-rest) | 0.994580 | 0.993885 |

<img width="890" height="340" alt="training_curve_gd" src="https://github.com/user-attachments/assets/3e12f13a-47a8-4d8a-95d2-d0336c27c970" />
<img width="851" height="390" alt="Confusion_Matrix" src="https://github.com/user-attachments/assets/23a5a4eb-f01b-46c4-888e-0bdb04db653f" />
<img width="890" height="390" alt="ROC_curve" src="https://github.com/user-attachments/assets/5773a3f1-bd2b-46d9-a25a-77b82dec8189" />
