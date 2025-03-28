# llama-fine-tuning
# Fine-tuning Llama-2 Model

This project fine-tunes the **Llama-2** model (7B parameters) on a custom dataset using **parameter-efficient fine-tuning** with **LoRA (Low-Rank Adaptation)**. The goal is to perform causal language modeling, i.e., text generation. The model is fine-tuned on the [Llama-2-SQL-Dataset](https://huggingface.co/datasets/ChrisHayduk/Llama-2-SQL-Dataset) for SQL-based question answering tasks.

## Requirements

Before running the code, make sure you have installed the required dependencies. The project uses the following libraries:
- **`datasets`**: For loading and processing datasets.
- **`transformers`**: For pre-trained models, tokenizers, and training utilities.
- **`peft`**: For parameter-efficient fine-tuning (LoRA).
- **`bitsandbytes`**: For efficient model quantization.
- **`torch`**: For deep learning operations.

## Installation

To set up the environment, use the following steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/llama-fine-tuning.git
    cd llama-fine-tuning
    ```

2. Create a virtual environment (recommended):

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use: venv\Scripts\activate
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### 1. Fine-tune the model:

To start fine-tuning the model on the custom dataset, run the `fine_tuning_llama.py` script:

```bash
python fine_tuning_llama.py
