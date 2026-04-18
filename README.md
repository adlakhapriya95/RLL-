# LLM Fine-Tuning using Direct Preference Optimization (DPO) for Reward-Aligned Text Generation

## Overview
This project demonstrates LLM fine-tuning using Direct Preference Optimization (DPO) with a small custom preference dataset and Hugging Face TRL. The objective is to align model outputs toward a campaign-style persuasive communication tone by training on prompt, chosen, and rejected response pairs.

The notebook uses `Qwen/Qwen2.5-0.5B-Instruct` as the base model and evaluates output quality before and after preference alignment.

The goal is to simulate how models can learn better decision-making strategies over time by optimizing for defined rewards.

---

## Problem Statement
Traditional machine learning models optimize for predefined labels, but many real-world problems require continuous improvement based on outcomes.

This project addresses:
- How to improve model decisions using feedback loops  
- How reward signals can guide better learning outcomes  
- How iterative fine-tuning compares to static training approaches  

---

## Approach

The project follows a reinforcement learning-based fine-tuning pipeline:

1. **Data Preparation**  
   - Input data is processed and structured for training  

2. **Model Training**  
   - Initial model is trained using a baseline approach  

3. **Reinforcement Learning Loop**  
   - Actions are evaluated using a reward function  
   - Model updates are guided by reward optimization  

4. **Fine-Tuning**  
   - Iterative updates improve model performance over time  

5. **Evaluation**  
   - Performance is measured across multiple iterations  
   - Comparison with baseline models  

---

## Key Concepts Used
- Reinforcement Learning (RL)
- Reward Optimization
- Model Fine-Tuning
- Iterative Training Pipelines
- Experimentation and Evaluation

---

## Tech Stack
- Python  
- Jupyter Notebook  
- Machine Learning / Reinforcement Learning libraries
- Json File for training the model 

---

## Results & Insights
- Demonstrates how reward-based learning improves model decisions over time  
- Highlights the importance of feedback loops in model optimization  
- Shows practical implementation of RL concepts in a structured pipeline  

---

## Why This Project Matters
This project reflects real-world AI system behavior where:
- Models must continuously learn from outcomes  
- Static training is not sufficient  
- Feedback-driven systems improve performance at scale  

It is especially relevant for:
- AI-driven products  
- Recommendation systems  
- Decision optimization systems  

---

## Future Improvements
- Hyperparameter tuning for better reward convergence  
- Scaling the pipeline for larger datasets  
- Integration with real-time feedback systems  
- Experiment tracking (MLflow or similar tools)  

---

## Author
**Priya Adlakha**  

Focus: Data-driven product development, AI systems, and end-to-end prototyping
