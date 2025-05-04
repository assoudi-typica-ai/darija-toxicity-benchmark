<p align="center">
  <img src="https://raw.githubusercontent.com/assoudi-typica-ai/darija-toxicity-benchmark/main/typicaai_logo.png" alt="Typica.ai Logo" width="200"/>
</p>

# A Comparative Benchmark of a Moroccan Darija Toxicity Detection Model (Typica.ai) and Major LLM-Based Moderation APIs (OpenAI, Mistral, Claude)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assoudi-typica-ai/darija-toxicity-benchmark/blob/main/eval_reproducibility.ipynb)

---

## 📄 Abstract

This repository accompanies the paper:

> **A Comparative Benchmark of a Moroccan Darija Toxicity Detection Model (Typica.ai) and Major LLM-Based Moderation APIs (OpenAI, Mistral, Claude)**  
> Hicham Assoudi  
> Typica.ai, Montreal, Canada

This paper presents a comparative benchmark evaluating the performance of Typica.ai’s custom Moroccan Darija toxicity detection model against major LLM-based moderation APIs: OpenAI (omni-moderation-latest), Mistral (mistral-moderation-latest), and Anthropic Claude (claude-3-haiku-20240307).

We focus on culturally grounded toxic content, including implicit insults, sarcasm, and culturally specific aggression often overlooked by general-purpose systems.  
Using a balanced test set derived from the **OMCD_Typica.ai_Mix** dataset, we report precision, recall, F1-score, and accuracy, offering insights into challenges and opportunities for moderation in underrepresented languages.  
Our results highlight Typica.ai’s superior performance, underlining the importance of culturally adapted models for reliable content moderation.

---

## 📦 Repository Contents

```
/data
  eval_baseline.csv
  final_evaluation_report.csv

/pred
  claud_results.csv
  mistral_results.csv
  openai_results.csv
  typica_ai_results.csv

typicaai_logo.png
eval_reproducibility.ipynb
LICENSE
README.md
```

---

## 🚀 How to Run

You can run this notebook manually in Google Colab without using a direct badge link:

1️⃣ **Download or Clone the Repository**  
- Download as ZIP and extract, or  
- Run:  
```bash
git clone https://github.com/assoudi-typica-ai/darija-toxicity-benchmark.git
```

2️⃣ **Open in Google Colab**  
- Go to [https://colab.research.google.com](https://colab.research.google.com)  
- Click **File → Upload Notebook**  
- Select `eval_reproducibility.ipynb` from the downloaded or cloned folder

3️⃣ **Install Requirements**  
- Colab will auto-install:
  - pandas
  - scikit-learn
  - altair
- If running locally, install with:
```bash
pip install pandas scikit-learn altair
```

4️⃣ **Run the Notebook**  
- Execute cells step by step:
  - Load and clean data
  - Merge predictions
  - Compute evaluation metrics
  - Visualize weighted F1 scores
  - Export final report

---

## 📜 License

This repository (code, notebook, paper, and datasets) is licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** License.

You are free to share and adapt the material for any purpose, even commercially, as long as you provide appropriate credit.

See [LICENSE](LICENSE) or visit [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) for details.

---

## 📚 Citation

If you use this work, please cite:

```
@article{assoudi2025moroccan,
  title={A Comparative Benchmark of a Moroccan Darija Toxicity Detection Model (Typica.ai) and Major LLM-Based Moderation APIs (OpenAI, Mistral, Claude)},
  author={Assoudi, Hicham},
  year={2025},
  publisher={Typica.ai}
}
```

---

## 💬 Contact

Hicham Assoudi  
Founder, Typica.ai  
📧 [assoudi@typica.ai](mailto:assoudi@typica.ai)
