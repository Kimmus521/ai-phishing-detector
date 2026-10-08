# AI Phishing Email Detector

A learning project that classifies emails as phishing or legitimate
and explains the signals behind each prediction.

## Problem Definition

Given one email file (.eml), classify it as phishing or legitimate
and show the signals that influenced the prediction.

## Planned Input and Output

- Input: One .eml email file.
- Output: Predicted class, model score, and supporting signals.
- Model scores will not be treated as calibrated probabilities
  unless calibration is evaluated.

## Evaluation

Primary metrics:
- Precision: How many emails flagged as phishing are actually phishing.
- Recall: How many actual phishing emails the model detects.

Additional metrics:
- F1 score
- Precision-recall AUC
- Confusion matrix

Numeric targets will be set after evaluating the baseline model.

## Data Policy

- Use public datasets and synthetic test emails.
- Keep raw emails and processed datasets out of Git.
- Record dataset sources, label definitions, and usage conditions.
- Do not treat every spam email as phishing.
- Do not open email links or execute attachments.

## Current Progress

- [x] Python virtual environment verified
- [x] Initial project structure prepared
- [x] Problem definition drafted
- [ ] Dataset sources and usage conditions reviewed
- [ ] Data collected and documented
- [ ] Email parsing and exploratory analysis completed
- [ ] Baseline model trained and evaluated

## Status

Development has started. No model has been trained or evaluated yet.
