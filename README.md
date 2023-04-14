# legal-instruct

*Idea behind the challenge*: 
Instruction finetuning large language models (LLMs) has shown huge potential (see for example the [Stanford Alpaca model](https://crfm.stanford.edu/2023/03/13/alpaca.html). By instruction tuning smaller LLMs, those models are able to solve complex tasks. Most LLMs have some legal texts in their trainingdata, but will often mix different legal sources in their outputs (especially for Switzerland this is an issue, because German texts for the Swiss legal system will often be mixed with legal information from Austria and Germany, for French and Italian it's the same issue). 

Creating a legal-instruct dataset based on Swiss data is essential for finetuning large language models (LLMs) that are used in the (swiss) legal industry. This dataset would contain legal instructions in a structured and organized format (following the alpaca format), if possible in German, French and Italian. It would allow LLMs to learn the language and nuances of our legal system and legal tasks. By having access to this comprehensive dataset, LLMs would be able to better understand legal language and improve their ability to accurately perform legal tasks.

Moreover, it is important that this dataset is openly available and allows for commercial use (the example of Alpaca is intended only for academic research and commercial use is prohibited). By creating an openly available and usable dataset, it would allow for broad implementation of the dataset and ensure that every open-source LLM could benefit from its use. This would not only benefit legal professionals (as many models could use that trainingdata freely) but also companies developing LLMs for the legal industry. An openly available legal-instruct dataset would also encourage collaboration and innovation in the field, ultimately leading to better outcomes for all.


## Goal of the challenge
* Create and release a legal-instruct dataset to huggingface with an open license.
* Finetune a LLM with the created dataset.

## Possible tasks:
* Writing clauses and legal texts
* Legal CoT (Chain of Thought) prompting
* QnA (simple or retrieval augmented)
* Summarization
* ...

## General Instruction Datasets:
[(Multilingual) Dataset for Dolly 2.0 from Databricks by Argila on Huggingface](https://huggingface.co/datasets/argilla/databricks-dolly-15k-multilingual)
