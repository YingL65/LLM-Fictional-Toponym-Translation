# LLM-Fictional-Toponym-Translation

Dataset and scripts for MPhil dissertation on LLM toponym translation experiments.

**1. Word Classifier**

This script automatically classifies compound words as either transparent or opaque. It splits an input word letter by letter from start to finish. If a split creates two parts that both appear in the COCA 20,000 frequency list, the word is classified as transparent. If the script checks every possible split and never finds a valid match for both parts, the word is classified as opaque.

**2. LLM Translation**

This script calls the ChatGPT API to translate the input text and asks the model to explain its translation choices (rationale). Due to the "black-box" nature of large language models, these generated explanations are not treated as direct proof of the model's internal reasoning process. Instead, they are used as supporting evidence to help analyze and understand the translation outputs.
