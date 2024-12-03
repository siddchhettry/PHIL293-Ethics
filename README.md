# Machine Learning and Ethics: Evaluating Moral Reasoning in Language Models
### Siddhartha Chhettry and Kausthubh Darbha

This repository contains the code and resources for the project **"Machine Learning and Ethics: Evaluating Moral Reasoning in Language Models"**, a class project for PHIL29300 at Purdue University. The project aims to compare how two different language models handle morally charged scenarios, exploring their alignment with human ethical standards.

## **Project Overview**

This project investigates the challenges of replicating human moral reasoning in AI systems. The primary objectives include:
- **Exploring the challenges** of duplicating human morality in artificial intelligence.
- **Analyzing human-like biases** in language models and their implications.
- **Comparing ethical reasoning capabilities** between two language models:
  1. Meta’s Llama 3.2 1B (standard)
  2. Meta’s Llama 3.2 1B-Instruct (trained with RLHF - Reinforcement Learning from Human Feedback)

### **Dataset**
The project uses the **ETHICS dataset** from Dan Hendrycks, Collin Burns, Steven Basart, Andrew Critch, Jerry Li, Dawn Song, and Jacob Steinhardt. It is a comprehensive resource for moral reasoning tasks. The dataset includes scenarios with human-assigned moral scores.
- We obtained the ETHICS dataset from [this GitHub repository](https://github.com/hendrycks/ethics) (which has been added to this repository for easier access).
- This dataset enables a quantitative comparison between human moral reasoning given by the dataset and the responses of the Llama language models.

---

## **Technical Approach**

The project uses a method inspired by Schramowski et al.'s paper (which can be found [here](https://doi.org/10.1038/s42256-022-00458-8)):
1. **Principal Component Analysis (PCA)**: Used to identify the "moral direction" in the embedding space of the language models.
2. **Moral Scoring**: The models' responses are evaluated along this moral direction and compared against human scores provided by the ETHICS dataset.
3. **Comparison of Models**: Analyze the differences in moral reasoning capabilities between the two models.
