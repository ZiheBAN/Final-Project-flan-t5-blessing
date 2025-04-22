# Final-Project-flan-t5-blessing
# Flan-T5 Fine-tuning for Blessing Message Generation

This project fine-tunes a Flan-T5-base model to generate personalized greeting messages (e.g., birthday wishes, anniversary notes, thank-you messages) using **hierarchical prompts**. The goal is to analyze how **prompt specificity** and **model fine-tuning** affect the output quality across fluency, relevance, and logical consistency.

---

## Project Structure

| File / Folder | Description |
|---------------|-------------|
| `Final Project.ipynb` | Main notebook containing data processing, model training, and generation workflows |
| `Final Report.pdf` | Final report in IEEE format summarizing the methodology, experiments, and results |
| `README.md` | Project overview and instructions (you’re reading it!) |
| `data/blessing_dataset_60_distinct_prompt.csv` | Manually constructed prompt-output training dataset (84 rows, 4 categories × 3 levels × 7 samples) |
| `evaluation/evaluation_template.csv` | Human evaluation of base model output |
| `evaluation/evaluation_template_finetuned.csv` | Human evaluation of fine-tuned model output |

---

## 🧠 Highlights

- **Model**: [Flan-T5-base](https://huggingface.co/google/flan-t5-base)
- **Training Samples**: 84 total (birthday, anniversary, encouragement, thank-you)
- **Prompt Levels**: Message-only → +Relation → +Detailed Context
- **Evaluation Dimensions**: Fluency, Relevance, Logic (scored 1–5 by human raters)
