<p align="center">
  <img src="https://raw.githubusercontent.com/assoudi-typica-ai/darija-toxicity-benchmark/main/typicaai_logo.png" alt="Typica.ai Logo" width="200"/>
</p>

> **This repository accompanies the paper:**

# A Comparative Benchmark of a Moroccan Darija Toxicity Detection Model (Typica.ai) and Major LLM-Based Moderation APIs (OpenAI, Mistral, Anthropic)
> Hicham Assoudi  
> Typica.ai, Montreal, Canada
---

## 📄 Abstract
This paper presents a comparative benchmark evaluating the performance of Typica.ai’s custom Moroccan Darija toxicity detection model against major LLM-based moderation APIs: OpenAI (omni-moderation-latest), Mistral (mistral-moderation-latest), and Anthropic Claude (claude-3-haiku-20240307).

We focus on culturally grounded toxic content, including implicit insults, sarcasm, and culturally specific aggression often overlooked by general-purpose systems.  
Using a balanced test set derived from the **OMCD_Typica.ai_Mix** dataset, we report precision, recall, F1-score, and accuracy, offering insights into challenges and opportunities for moderation in underrepresented languages.  
Our results highlight Typica.ai’s superior performance, underlining the importance of culturally adapted models for reliable content moderation.

---

## 📊 Evaluation Results

Here’s the final weighted F1-score comparison graph:

<p align="center">
  <img src="https://raw.githubusercontent.com/assoudi-typica-ai/darija-toxicity-benchmark/main/eval_visualization.png" alt="Evaluation Visualization" width="600"/>
</p>

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

eval_reproducibility.ipynb
LICENSE
README.md
```

---

## 🚀 How to Run

You can run this notebook using the Colab badge, but note that you will need to provide the required `data/` and `pred/` files.

1️⃣ **Download the Repository Files**  
- Download this repository as a ZIP and extract it, or  
- Clone it using:
```bash
git clone https://github.com/assoudi-typica-ai/darija-toxicity-benchmark.git
```

---

2️⃣ **Launch Notebook in Colab**
- Use the Colab badge below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assoudi-typica-ai/darija-toxicity-benchmark/blob/main/eval_reproducibility.ipynb)

---

3️⃣ **Upload Required Files in Colab**
- Once inside Colab, manually upload the contents of:
  - `/data` → CSV files  
  - `/pred` → CSV files

You can do this via the **Colab file browser sidebar** → **Upload**.

---

4️⃣ **Install Requirements (Handled in Colab)**
The notebook automatically installs:
- pandas
- scikit-learn
- altair

If running locally, you can install them using:
```bash
pip install pandas scikit-learn altair
```

---

5️⃣ **Run the Notebook**
- Execute the cells step by step to:
  - Load and clean data
  - Merge predictions
  - Compute evaluation metrics
  - Visualize weighted F1 scores
  - Export the final report
    
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
