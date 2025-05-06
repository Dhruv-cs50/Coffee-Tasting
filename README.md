# Great American Coffee Taste Test Analysis

**Authors:** James Kim, Dhruv Shah, Sang Tran  
**Date:** April 29th, 2025

---

## 📖 Project Overview

The Great American Coffee Taste Test project investigates how roast level, demographics, and self-reported preferences influence blind-taste coffee choices. Using a 4,000-participant dataset collected via a livestream tasting by James Hoffmann and Cometeer, we explore:

1. **Overall Preference Patterns:** Which of the four samples (A: light roast, B: medium roast, C: dark roast, D: experimental Colombian) is most enjoyed?  
2. **Demographic Correlates:** How do age, gender, and coffee-drinking habits relate to blind-taste favorites?  
3. **Self-Report vs. Reality:** Do people’s stated roast preferences align with their blind-taste picks?  
4. **Qualitative Notes:** What tasting-note keywords explain unexpected favorites?

---

## 📂 Repository Structure

coffee_taste_test/
├── data/
│   ├── raw/
│   │   └── GACTT_RESULTS_ANONYMIZED_v2.csv
│   └── clean/
│       ├── cleaned_core.csv
│       └── cleaned_with_notes.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploratory_analysis.ipynb
│   ├── 03_statistical_tests.ipynb
│   └── 04_machine_learning_models.ipynb
├── src/
│   ├── clean.py
│   ├── eda.py
│   └── stats.py
├── output/
│   ├── figures/
│   └── tables/
├── requirements.txt
└── README.md

- **data/raw/**: original dataset files  
- **data/clean/**: cleaned CSVs with selected columns and normalized fields  
- **notebooks/**: Jupyter notebooks for each analysis step  
- **src/**: helper modules for cleaning, EDA, and statistical tests  
- **output/**: generated figures and summary tables  
- **requirements.txt**: Python dependencies  

---

## 🚀 Getting Started

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/coffee_taste_test.git
   cd coffee_taste_test

	2.	Create and activate a virtual environment

python3 -m venv venv
source venv/bin/activate


	3.	Install dependencies

pip install -r requirements.txt


	4.	Run the analysis notebooks in order
	1.	01_data_cleaning.ipynb → produces cleaned_core.csv and cleaned_with_notes.csv
	2.	02_exploratory_analysis.ipynb → generates EDA plots in output/figures
	3.	03_statistical_tests.ipynb → computes chi-square tests and roast-alignment rates
	4.	04_tasting_notes.ipynb → extracts and visualizes top tasting-note keywords

⸻

📊 Key Findings
	•	Coffee D was the runaway favorite (1,382 picks), outperforming the Kenyan roast series (A/B/C ~800 each).
	•	Demographics matter: Both age and gender show statistically significant associations with sample choice (p < 0.001).
	•	Self-report gap: Only ~27.5% of participants correctly predicted their blind-taste favorite after normalizing variants (“Blonde” → Light, etc.).
	•	Flavor drivers: Among “surprised” tasters, “fruity,” “smooth,” and “bitter” were the most common descriptors—highlighting how flavor characteristics can override roast expectations.

⸻

⚠️ Limitations
	•	Sample bias: Participants were specialty-coffee enthusiasts, not a random cross-section of Americans.
	•	Missing data: Some demographic and tasting-note fields were sparsely populated.
	•	Simplistic text analysis: We used basic keyword counts; more advanced NLP could yield deeper insights.

⸻

🤝 Contributing
	1.	Fork this repository
	2.	Create a feature branch:

git checkout -b feature/my-analysis


	3.	Commit your changes:

git commit -m "Add advanced NLP analysis"


	4.	Push to your branch:

git push origin feature/my-analysis


	5.	Open a Pull Request for review

⸻

📜 License

This project is licensed under the MIT License. See LICENSE for details.

