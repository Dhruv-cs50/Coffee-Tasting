# Great American Coffee Taste Test Analysis

**Authors:** James Kim, Dhruv Shah, Sang Tran  
**Date:** Spring 2025

---

## 📖 Project Overview

The Great American Coffee Taste Test project investigates how roast level, demographics, and self‐reported preferences influence blind‐taste coffee choices. Using a 4,000-participant dataset collected via a livestream tasting by James Hoffmann and Cometeer, we explore:

1. **Overall Preference Patterns:** Which of the four samples (A: light roast, B: medium, C: dark, D: experimental Colombian) is most enjoyed?  
2. **Demographic Correlates:** How do age, gender, and coffee‐drinking habits relate to blind‐taste favorites?  
3. **Self-Report vs. Reality:** Do people’s stated roast preferences align with their blind‐taste picks?  
4. **Qualitative Notes:** What tasting‐note keywords explain unexpected favorites?

---

## 📂 Repository Structure

coffee_taste_test/
├── data/
│   ├── raw/                     # Original CSV downloads
│   │   └── GACTT_RESULTS_ANONYMIZED_v2.csv
│   └── clean/                   # Processed CSVs
│       ├── cleaned_core.csv     # Core columns cleaned
│       └── cleaned_with_notes.csv  # Includes tasting notes & normalized fields
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploratory_analysis.ipynb
│   ├── 03_statistical_tests.ipynb
│   └── 04_tasting_notes.ipynb   # Qualitative keyword analysis
├── src/
│   ├── clean.py                 # Cleaning & normalization functions
│   ├── eda.py                   # Plotting & summary functions
│   └── stats.py                 # Chi-square, alignment, keyword‐count utilities
├── output/
│   ├── figures/                 # PNGs of all charts
│   └── tables/                  # CSV or markdown tables of results
└── README.md                    # This file

---

## 🚀 Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/coffee_taste_test.git
   cd coffee_taste_test

	2.	Create a virtual environment & install dependencies

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt


	3.	Run the notebooks in order
	•	01_data_cleaning.ipynb → produce cleaned_core.csv and cleaned_with_notes.csv.
	•	02_exploratory_analysis.ipynb → generate EDA plots in output/figures.
	•	03_statistical_tests.ipynb → compute chi‐square results & roast‐alignment rates.
	•	04_tasting_notes.ipynb → extract and plot top tasting‐note keywords.

⸻

📊 Key Findings
	•	Coffee D was the runaway favorite (1,382 picks), outperforming the Kenyan roast series (A/B/C ~800 each).
	•	Demographics matter: Both age and gender showed statistically significant associations with sample choice (p < 0.001).
	•	Self-report gap: Only ~27.5% of participants correctly predicted their blind‐tasting favorite after normalizing “Blonde”→Light, etc.
	•	Flavor drivers: Among surprised tasters, “fruity,” “smooth,” and “bitter” were the most common descriptors—highlighting how flavor notes can override roast expectations.

⸻

⚠️ Limitations
	•	Sample bias: Participants were specialty‐coffee enthusiasts, not a random cross-section of Americans.
	•	Missing data: Some demographic and free‐text fields were sparsely populated.
	•	Text analysis simplicity: We used basic token counts; more advanced NLP could reveal deeper themes.

⸻

🤝 Contributing
	1.	Fork this repository
	2.	Create a feature branch (git checkout -b feature/my-analysis)
	3.	Commit your changes (git commit -m "Add advanced NLP analysis")
	4.	Push to your branch (git push origin feature/my-analysis)
	5.	Open a Pull Request for review

⸻

📜 License

This project is released under the MIT License. See LICENSE for details.

⸻

— Dhruv Shah and Team
