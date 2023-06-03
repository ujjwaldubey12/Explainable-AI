# Explainable-AI-Project

# Can Explanations Unveil Bias in AI Systems?

**Affiliation:** Luddy School of Informatics, Computing, and Engineering, Indiana University, Bloomington

![shap](https://github.com/ujjwaldubey12/Explainable-AI/assets/135392087/afe7b56e-b9ca-4093-a2b5-efa88fc24ac8)

## Abstract
The ethical implications and fairness in the AI industry have been subjects of ongoing debate. This project aims to explore whether explainable AI can shed light on fairness issues. We analyze the COMPAS dataset and employ explainable AI tools to investigate if explanations can reveal the bias present in the system.

## Introduction
The challenge of determining who complies with the law and who does not has become more complex with the advancements in Machine Learning and Artificial Intelligence. Risk assessment algorithms, such as COMPAS (Correctional Offender Management Profiling for Alternative Sanctions), are increasingly being used by judges and parole officials to predict recidivism. However, studies have shown that the COMPAS algorithm exhibits bias in favor of white defendants and against black convicts. In this paper, we focus on the COMPAS dataset and utilize explainable AI tools to assess the presence of bias and examine its impact.

## Motivation
AI-based algorithms can assist in decision-making, but their inner workings are often difficult for humans to understand. Explainable AI (XAI) aims to provide explanations for the decisions made by AI models and identify the factors that influence those decisions. XAI can also contribute to evaluating the fairness of AI models, thereby building trust in AI/ML systems. By enhancing interpretability, XAI can drive the development of ethical and responsible AI.

## Methodology
We begin by analyzing the COMPAS dataset from an ethical perspective, as biased datasets tend to produce biased predictions. We modify the column feature names to align with ethical standards while retaining sufficient information for accuracy and fairness analysis using SHAP (SHapley Additive exPlanations) and WIT (What-If Tool).

We employ three classification methods: Logistic Regression, Random Forest, and Deep Neural Network, to predict the likelihood of re-offending. We then incorporate explainability using ad hoc explanations, SHAP, LIME (Local Interpretable Model-Agnostic Explanations), and WIT. These tools help us understand the decisions made by the models, assess accuracy and fairness, and analyze feature importance.

## Results and Discussion
In the Logistic Regression model, features such as Ethnic Code Text and Scale ID show the most negative weights, while RawScore and RecSupervisionLevelText exhibit the most positive weights in predicting the score text. The Confusion Matrix indicates some bias in the model, with false positives for African-American defendants. However, the Random Forest model performs better and reduces false positives significantly.

We utilize LIME for local explanations, providing insights into specific attribute influences on the model's predictions. Additionally, we focus on the analysis provided by the What-If Tool (WIT) to evaluate the model's performance and fairness from a human-centered perspective.

## Conclusion
This study investigates the potential of explainable AI in uncovering bias in AI systems. By analyzing the COMPAS dataset and employing various XAI tools, we demonstrate the effect of explanations on the fairness of AI models. Our findings emphasize the importance of transparency and interpretability in AI to ensure ethical and responsible AI practices.

## Literature Review
The paper "Can Explainable AI Explain Unfairness? A Framework for Evaluating Explainable AI" introduces a rubric to assist XAI in explaining fairness issues. It also discusses the apparent conflict between individual and group fairness and presents three XAI tools: LIME, AI Explainability 360, and ad-hoc explainability tools.

Another study, "Transparency in Fair Machine Learning: The Case of Explainable Recommender Systems," highlights various biases that can infiltrate AI systems such as algorithmic bias and recommendation bias. It emphasizes the importance of transparency in explainable recommender systems to address these biases and promote fairness.

The research article "Interpretable Machine Learning: Definitions, Methods, and Applications" provides an overview of interpretability techniques in machine learning, including rule-based models, tree-based models, and model-agnostic approaches. It discusses the benefits of interpretability in building trust and understanding complex AI systems.

In the paper "Fairness and Transparency in Machine Learning for Human Health," the authors explore the impact of bias in healthcare AI systems and the role of transparency and interpretability in addressing these issues. They emphasize the need for explainable AI to ensure fair and accountable decision-making in healthcare.

Another relevant study, "Explaining Explainability: A Systematic Review of Explainable Artificial Intelligence Literature," conducts a comprehensive review of explainable AI literature and provides insights into the current state of research, challenges, and future directions. It covers various aspects of explainability, including model-agnostic and model-specific approaches, interpretability techniques, and evaluation methods.

These studies collectively contribute to the understanding of the role of explainable AI in uncovering bias and promoting fairness in AI systems. They highlight the significance of transparency, interpretability, and ethical considerations in the development and deployment of AI technologies. By leveraging explainable AI tools and methodologies, researchers and practitioners can gain insights into the decision-making processes of AI models and mitigate the potential biases that might arise.
