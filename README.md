# LLM Fine-Tuning using Direct Preference Optimization (DPO) for Reward-Aligned Text Generation

## Overview
This project demonstrates LLM fine-tuning using Direct Preference Optimization (DPO) with a custom preference dataset and Hugging Face TRL. The objective is to align model outputs toward a campaign-style persuasive communication tone by training on prompt, chosen, and rejected response pairs.

The notebook uses `Qwen/Qwen2.5-0.5B-Instruct` as the base model and evaluates output quality before and after preference alignment.

The goal is to improve model behavior by optimizing outputs based on preference comparisons rather than traditional supervised learning.

---

## Problem Statement
Large Language Models often generate outputs that are not aligned with desired tone, intent, or user expectations. Standard supervised fine-tuning does not fully capture nuanced preferences such as style, persuasion, or communication effectiveness.

This project addresses:
- How to align LLM outputs using preference-based learning  
- How pairwise comparisons (chosen vs rejected responses) improve output quality  
- How iterative fine-tuning can enhance stylistic consistency and decision-making  

---

## Approach

The project follows a preference-based fine-tuning pipeline:

1. **Data Preparation**  
   - Custom dataset structured with `prompt`, `chosen`, and `rejected` responses  
   - JSON-based format for training  

2. **Base Model Setup**  
   - Pretrained model: `Qwen/Qwen2.5-0.5B-Instruct`  
   - Loaded using Hugging Face Transformers  

3. **Preference Optimization (DPO)**  
   - Direct Preference Optimization used to align outputs  
   - Learns from pairwise comparisons without explicit reward modeling  
   - Implemented using Hugging Face TRL (`DPOTrainer`)  

4. **Fine-Tuning**  
   - Model updated iteratively using preference signals  
   - Hyperparameters such as beta and learning rate explored  

5. **Evaluation**  
   - Comparison of model outputs before and after fine-tuning  
   - Qualitative assessment of tone, persuasion, and alignment  

---

## Key Concepts Used
- Large Language Model (LLM) Fine-Tuning  
- Direct Preference Optimization (DPO)  
- Preference-Based Learning  
- Model Alignment  
- Iterative Training Pipelines  

---

## Tech Stack
- Python  
- Jupyter Notebook  
- Hugging Face Transformers  
- TRL (Transformer Reinforcement Learning Library)  
- JSON-based dataset  

---

## Results & Insights
- Improved alignment toward persuasive, campaign-style communication after fine-tuning  
- Clear differences observed between pre-trained and fine-tuned model outputs  
- Hyperparameter tuning (beta, learning rate) impacts output quality and consistency  
- Demonstrates effectiveness of preference-based training without explicit reward models  

---

## Why This Project Matters
This project reflects how modern AI systems are aligned with human preferences in real-world applications.

It is especially relevant for:
- AI-driven products  
- Conversational AI and chat systems  
- Content generation and personalization  
- LLM alignment and safety research  

---

## Future Improvements
- Expand dataset for better generalization  
- Quantitative evaluation metrics (BLEU, ROUGE, or human evaluation)  
- Integration with real-time feedback systems  
- Experiment tracking using MLflow or similar tools  

---

## Author
**Priya Adlakha**  

Focus: Data-driven product development, AI systems, and end-to-end prototyping
