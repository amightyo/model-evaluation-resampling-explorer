# Model Evaluation & Resampling Explorer

An interactive learning tool for exploring how train/test splits, sampling variability, and cross-validation affect estimates of machine learning model performance.

🔗 **Live Explorer:**  
https://amightyo.github.io/model-evaluation-resampling-explorer/

## Why This Explorer?

A machine learning model may achieve 84% accuracy on one train/test split and 91% on another.

Which number represents the model's performance?

The Model Evaluation & Resampling Explorer helps learners investigate this question interactively rather than simply accepting a single performance estimate.

The central idea is:

> A single performance score is an estimate—not an intrinsic property of a modeling procedure.

## Learning Experience

The explorer guides learners through a progressive experiment:

**See the Data → Split It → Fit → Evaluate → Re-Split → Observe Variability → Examine a Distribution → Cross-Validate → Make an Evaluation Decision**

Learners investigate:

- training and test sets;
- the purpose of a random state or seed;
- variability across train/test splits;
- distributions of performance estimates;
- mean performance and variability;
- 5-fold cross-validation;
- data leakage;
- evaluation considerations for imbalanced, temporal, and grouped data; and
- the distinction between a modeling procedure and a fitted model.

## Key Teaching Principle

The explorer deliberately keeps the dataset, target, predictors, algorithm, model settings, and train/test ratio fixed while changing which observations are assigned to training and testing.

This allows learners to ask:

> **If the modeling procedure did not change, why did the estimated performance change?**

The goal is not to search for the random seed that produces the highest score. The goal is to understand uncertainty in model evaluation.

## Using the Explorer

No installation is required.

Open the live explorer:

https://amightyo.github.io/model-evaluation-resampling-explorer/

You can also download or clone this repository and open `index.html` in any modern web browser.

## Teaching With the Explorer

One possible classroom sequence is:

1. Ask students whether one test-set score is enough to describe model performance.
2. Run the first 80/20 train/test split.
3. Re-split the same data and compare the new performance estimate.
4. Repeat the experiment several times.
5. Examine the distribution, mean, standard deviation, and range.
6. Introduce cross-validation as a systematic resampling strategy.
7. Discuss whether the evaluation design matches the real-world prediction problem.
8. Ask students to design and defend an evaluation strategy for their own project.

## LMS / Canvas

Because the explorer is hosted with GitHub Pages, it can be embedded in an LMS such as Canvas using an iframe.

```html
<iframe
  src="https://amightyo.github.io/model-evaluation-resampling-explorer/"
  title="Model Evaluation and Resampling Explorer"
  width="100%"
  height="2500"
  style="border: 1px solid #d9e4e1; border-radius: 8px;"
  loading="lazy"
  allowfullscreen>
</iframe>
```

If your LMS restricts embedded content, link directly to the GitHub Pages version.

## Course Context

This explorer was developed for ANLY 530: Principles and Applications of Machine Learning at Harrisburg University as part of an applied, problem-first approach to teaching machine learning.

The instructional philosophy is:

> Problem First. Model Second. Evaluation before celebration.

## Author

Itauma Itauma, PhD
Associate Professor of Data Science & Analytics
Harrisburg University

Website: https://amightyo.github.io/

License

This project is released under the MIT License. See LICENSE for details.
