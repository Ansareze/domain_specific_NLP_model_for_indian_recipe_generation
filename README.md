# Domain-Specific NLP Model for Indian Recipe Generation

This project focuses on fine-tuning a pretrained NLP model to generate step-by-step Indian food recipes based on user queries. It demonstrates how domain adaptation can be used to train models for highly specific tasks like recipe generation.

---

## 📌 Objective

To build a text generation model that responds to user prompts like:

> “How to make Paneer Butter Masala?”  
> “Give me the steps to prepare Dosa.”

And returns structured, human-readable recipes with ingredients and instructions.

---

## 📂 Dataset

- **Source:** Curated dataset of Indian recipes
- **Format:** Text-based records including title, ingredients, and step-wise instructions
- **Structure:**
  - `title`: Name of the dish
  - `ingredients`: List of ingredients
  - `steps`: Sequential instructions

---

## 🔧 Model & Approach

- **Base Model:** Pretrained Transformer (e.g., GPT-2, T5, or similar)
- **Technique:** Fine-tuning via supervised learning
- **Training Pipeline:**
  - Tokenization using HuggingFace Tokenizer
  - Input-output pairs created as (prompt → recipe)
  - Trained with teacher forcing and cross-entropy loss

---

## 🚀 Features

- Prompt-based generation (e.g., "How to make [dish]?")
- Step-by-step output structure
- Domain-specific language modeling
- Transfer learning for real-world application

---

## 🧠 Key Learnings

- Domain-specific NLP fine-tuning
- Prompt engineering for sequence generation
- Evaluation of generation quality (BLEU, manual inspection)
- Exposure to real-world text generation workflows

---

## 📊 Example Output

**Input Prompt:**  
`How to make Rajma Chawal?`

**Generated Output:**  
