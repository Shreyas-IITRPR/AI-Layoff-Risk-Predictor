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
