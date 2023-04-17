# legal-instruct

*💡 Idea behind the challenge*: 

Instruction finetuning large language models (LLMs) has shown huge potential (see InstructGPT by OpenAI[^1]) this has further been improved by synthetically generated instructions using the [self instruct](https://arxiv.org/abs/2212.10560)[^2] method (see for example the [Stanford Alpaca model](https://crfm.stanford.edu/2023/03/13/alpaca.html). By instruction tuning smaller LLMs, those models are able to solve complex tasks. Most LLMs have some legal texts in their trainingdata, but will often mix different legal sources in their outputs (especially for Switzerland this is an issue, because German texts for the Swiss legal system will often be mixed with legal information from Austria and Germany, for French and Italian it's the same issue). Generating synthetic data is (apart from API usage limitations by for example OpenAI) therefore also not possible in the legal domain, as those _mixtures_ would be present in the generated data as well. 

Creating a legal-instruct dataset based on Swiss data is essential for finetuning large language models (LLMs) that are used in the (swiss) legal industry. This dataset would contain legal instructions in a structured and organized format (following the alpaca format), if possible in German, French and Italian. It would allow LLMs to learn the language and nuances of our legal system and legal tasks. By having access to this comprehensive dataset, LLMs would be able to better understand legal language and improve their ability to accurately perform legal tasks.

Moreover, it is important that this dataset is openly available and allows for commercial use (the example of Alpaca is intended only for academic research and commercial use is prohibited). By creating an openly available and usable dataset, it would allow for broad implementation of the dataset and ensure that every open-source LLM could benefit from its use. This would not only benefit legal professionals (as many models could use that trainingdata freely) but also companies developing LLMs for the legal industry. An openly available legal-instruct dataset would also encourage collaboration and innovation in the field, ultimately leading to better outcomes for all.


## 🎯 Goal of the challenge
* Create and release a legal-instruct dataset to huggingface with an open license.
* Finetune a LLM with the created dataset.

## Possible tasks:
* Writing clauses and legal texts
* Legal CoT (Chain of Thought) prompting
* QnA (simple or retrieval augmented)
* Summarization
* ...

## Roadmap

This will have to be discussed at the hackathon. 

- [x] Simple platform to collect data (already in progess).
- [ ] Datacollection. 
- [ ] Define a (very) simple benchmark to see what outputs would be considered as _good_ or _bad_.
- [ ] Select suitable LLM to finetune ([Dolly 2.0](https://huggingface.co/databricks/dolly-v2-7b), [Open Assistant (Pythia base)](https://huggingface.co/OpenAssistant), [T0pp](https://huggingface.co/bigscience/T0pp) or [FLAN-ul2](https://huggingface.co/google/flan-ul2)) 
- [ ] Finetuning an LLM (LoRA finetuning, as  this could probably be acheived in the limitted time of the hackathon and wouldn't need expensive hardware).
- [ ] Review of the model.

# Available Data

## General (multilingual) Instruction Datasets:
[Dataset for Dolly 2.0 from Databricks by Argila on Huggingface](https://huggingface.co/datasets/argilla/databricks-dolly-15k-multilingual)

[OpenAssistant Conversations Dataset (OASST1) by Open Assistant on Huggingface](https://huggingface.co/datasets/OpenAssistant/oasst1)

---

# Citations
[^1]: Ouyang, Long, Jeff Wu, Xu Jiang, Diogo Almeida, Carroll L. Wainwright, Pamela Mishkin, Chong Zhang, et al. *‘Training Language Models to Follow Instructions with Human Feedback’*. ArXiv [Cs.CL], 2022. arXiv. [http://arxiv.org/abs/2203.02155](http://arxiv.org/abs/2203.02155). And [OpenAI Blog (last visitted on Mon. 17th of April 2023)](https://openai.com/research/instruction-following)

[^2]: Wang, Yizhong, Yeganeh Kordi, Swaroop Mishra, Alisa Liu, Noah A. Smith, Daniel Khashabi, and Hannaneh Hajishirzi. ‘Self-Instruct: Aligning Language Model with Self Generated Instructions’. ArXiv [Cs.CL], 2022. arXiv. [http://arxiv.org/abs/2212.10560](http://arxiv.org/abs/2212.10560).
