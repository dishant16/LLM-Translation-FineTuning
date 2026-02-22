# LLM Fine-Tuning for German-to-French Translation

This project focuses on fine-tuning a Large Language Model (LLM) to perform high-quality translation using memory-efficient techniques.

## 🚀 Project Overview
* **Model:** FLAN-T5-XL (3B Parameters)
* **Objective:** Improve German-to-French translation accuracy.
* **Key Techniques:** * **LoRA (Low-Rank Adaptation):** Efficiently fine-tuned parameters without updating the entire model.
    * **4-bit Quantization (bitsandbytes):** Reduced memory footprint to run on consumer-grade GPUs.
    * **Knowledge Distillation:** Generated 1,600 high-quality synthetic translation pairs using **Mixtral-8x7B** via Groq API.


## 🛠️ Tech Stack
* **Frameworks:** PyTorch, Hugging Face (Transformers, PEFT, Accelerate)
* **Libraries:** Bitsandbytes (Quantization), Evaluate (Metrics)
* **API:** Groq (Mixtral-8x7B for data augmentation)
* **Language:** Python

## 📖 How to Use
1. Install dependencies: `pip install -r requirements.txt`
2. Run inference: `python src/inference.py --text "Guten Morgen"`
