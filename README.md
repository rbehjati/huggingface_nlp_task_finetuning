# HuggingFace NLP Tasks FineTuning Notebooks

This repository contains notebooks which show how to finetune language models using the HuggingFace Libraries. There are 6 main NLP tasks which have their own notebook:

1. Causal Language Modelling: Given a sequence of text, predict the next tokens in the sequence.
2. Masked Language Modelling: Given a sequence of text, mask out particular tokens and predict those masked tokens.
3. Translation: Translate a sequence of text from a source language to a target language.
4. Summarisation: Given a sequence of text, produce a shortened sequence that summarises the longer sequences.
5. Token Classification: Named entity recognition within a sequence.
6. Question Answering: Given a sequence of text which is an instruction/ question and some context provided, generate a sequence of text that answers that question using the context.

These notebooks all require GPUs for training, hence it is advised to run them with Google Colab. 

There are 3 subdirectories in this repository:

1. `trainer`: Finetunes model using the HuggingFace Trainer API - represents the most straightforward way of model finetuning.
2. `PyTorch`: Trainer API is largely build on top of PyTorch. These notebooks show how to finetune models using a PyTorch training loop without relying on the Trainer API.
3. `PEFT`: Finetuning models using the HuggingFace Trainer API and using the PEFT library to introduce and finetune LoRA (Low Rank Adaptation) Adapters.

**Note**: These Notebooks mirror the official HuggingFace Transformers Docs with additional code for clarification. It is more than possible that there is some erroneous or superfluous code in the Notebooks. If seen, please make a Github issue with this repo and I will correct them.


# References

1. [HuggingFace Transformers Main NLP Tasks](https://huggingface.co/learn/nlp-course/chapter7/1)
2. [Parameter Efficient Fine Tuning](https://huggingface.co/blog/peft)
3. [Transformers and Large Language Models Study List](https://paper.dropbox.com/doc/Transformers-and-Large-Language-Model-Study-List--B~xlppzcQnErugHV_HWCJC9yAg-5pNgAe0SG2beUMdKYfRZv)
4. [Create a Training Loop for PyTorch Models](https://machinelearningmastery.com/creating-a-training-loop-for-pytorch-models/)