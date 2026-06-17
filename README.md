# Email Generation Assistant

An AI-powered email generation assistant built with Groq LLaMA models.

## Setup
1. Install dependencies: pip install groq pandas
2. Get free API key from: https://console.groq.com
3. Paste your key in Cell 2

## How to Run
Open the notebook in Google Colab and run all cells in order.

## Advanced Prompting Technique
Role-Playing + Few-Shot Examples + Chain-of-Thought prompting
using Alexandra Chen persona with 2 few-shot examples and
a 4-step internal reasoning process.

## Custom Evaluation Metrics
1. Fact Recall — % of key facts found in generated email
2. Tone Accuracy — LLM-as-a-Judge score (0 to 1)
3. Conciseness — Word count penalty score

## Results
| Model | Fact Recall | Tone Accuracy | Conciseness | Average |
|-------|-------------|---------------|-------------|---------|
| llama-3.3-70b-versatile | 1.00 | 0.91 | 0.96 | 0.96 |
| llama-3.1-8b-instant | 1.00 | 0.91 | 0.96 | 0.96 |

## Recommendation
Model B (8b-instant) recommended for production — identical
quality at faster speed and lower cost.

## Deliverables
- email_assistant.ipynb — Full notebook with all code
- evaluation_results.csv — Raw scores for all 10 scenarios
- analysis_report.txt — Comparative analysis report
