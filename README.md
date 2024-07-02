# ELMo: Deep Contextualized Word Representations

## About the Project
This project focuses on building and pretraining an ELMo (Embeddings from Language Models) architecture using PyTorch. ELMo provides deep contextualized word representations that capture syntactic and semantic meanings of words in context, which are beneficial for various NLP tasks. The project includes pretraining the ELMo model and evaluating its performance on a downstream classification task.

## Pretrained Embeddings
The initial input embeddings for ELMo are derived from the `glove.6B.100d` embeddings. These embeddings can be easily downloaded from the internet by searching for "glove.6B.100d".

## Steps to Run

1. **Run the ELMo Pretraining:**
    - Execute the `elmo-pretraining.ipynb` notebook.
    - This notebook will train the ELMo model and produce 3 models, each corresponding to different hyperparameter settings mentioned in the assignment PDF.
        - **Hyperparameter 1: Trainable λs**
            - In this setting, λs are trainable parameters that are learned during training.
        - **Hyperparameter 2: Frozen λs**
            - In this setting, λs are randomly initialized and kept frozen during training.
        - **Hyperparameter 3: Learnable Function**
            - In this setting, a function is learned to combine word representations across layers to build the final contextual word embedding.

2. **Run the Classification Task:**
    - Execute the `classification-task.ipynb` notebook.
    - This notebook will train and evaluate each of the pretrained ELMo models on the AG News Classification Dataset.

## Additional Information
Ensure that you have the following files and dependencies in place to run the notebooks:
- Python
- PyTorch
- Jupyter Notebook
- The AG News Classification Dataset
- Pretrained `glove.6B.100d` embeddings

Follow the instructions in each notebook for detailed steps and code execution.

---
