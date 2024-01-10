# | NLP | PPO | DialogSum | Less-Toxic Summarize |

## NLP (Natural Language Processing) with PEFT (Parameter Efficient Fine-Tuning) and LoRA (Low-Rank Adaptation) for Less-Toxic Summarization

# <b><span style='color:#78D118'>|</span> Introduction</b>

This project explores the capabilities of Large Language Models (LLMs), particularly emphasizing the utilization of Parameter Efficient Fine-Tuning (PEFT) to create dialogue summaries with reduced toxicity. We achieve this by employing the FLAN-T5 model alongside Meta AI's hate speech reward model.

Our primary objective is to improve the quality of dialogue summaries while minimizing toxicity. To attain this, we apply Proximal Policy Optimization (PPO) for fine-tuning, aiming to mitigate the model's toxic output. Furthermore, we will showcase the advantages of Parameter Efficient Fine-Tuning (PEFT), illustrating that its benefits surpass any potential minor performance trade-offs.

 - NOTE: This is an example and we not using the entirety of the data used.
 
## Objectives :
 - Train LLM to make less toxic dialogue summarization.
 
 
 ## The DialogSum Dataset:
The [DialogSum Dataset](https://huggingface.co/datasets/knkarthick/dialogsum) DialogSum is a large-scale dialogue summarization dataset, consisting of 13,460 (Plus 100 holdout data for topic generation) dialogues with corresponding manually labeled summaries and topics.

## Project Workflow:

- **Setup**: Import necessary libraries and define project parameters.
- **Dataset Exploration**: Discovering DialogSum Dataset.
- **Test Model Zero Shot Inferencing**: Initially, test the FLAN-T5 model for zero-shot inferencing on dialogue summarization tasks to establish a baseline performance.
- **Dataset Preprocess Dialog and Summary**: Preprocess the dialog and its corresponding summary from the dataset to prepare for the train.
-  **Perform Parameter Efficient Fine-Tuning (PEFT)**: Implement Parameter Efficient Fine-Tuning (PEFT), a more efficient fine-tuning approach that can significantly reduce training time while maintaining performance.
-  **Evaluation**:
    - Perform human evaluation to gauge the model's output in terms of readability and coherence. This can involve annotators ranking generated summaries for quality.
    - Utilize ROUGE metrics to assess the quality of the generated summaries. ROUGE measures the overlap between generated summaries and human-written references.

[| View on Kaggle |](kaggle.com/code/yannicksteph/nlp-ppo-dialogsum-less-toxic-summarize/notebook)
