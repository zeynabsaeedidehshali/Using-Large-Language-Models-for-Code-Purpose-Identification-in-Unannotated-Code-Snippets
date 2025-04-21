Using Large Language Models for Code Purpose Identification in Unannotated Code Snippets
This project explores how we can use Large Language Models (LLMs) like StarCoder, StableCode 3B, and Llama 3.2 to figure out the purpose of uncommented code — basically trying to make sense of functions that don’t have any documentation.
I evaluated these models in a zero-shot setting, using prompts like “Explain what this code does” without giving them examples or training. The goal was to see how well they could generate human-like explanations.
Datasets Used:
- CodeSearchNet (Java + Python)
- CoNaLa (Python)
Models Tested:
- StarCoder
- StableCode 3B
- Llama 3.2
Evaluation Metrics:
- BLEU-2
- ROUGE
- METEOR
- Cosine Similarity
Summary:
- StableCode 3B gave the most consistent results across tasks
- StarCoder performed best on Python with CoNaLa
- Llama 3.2 wasn’t trained specifically on code but still did well semantically
