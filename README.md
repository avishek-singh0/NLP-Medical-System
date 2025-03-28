# NLP-Medical-System

This project leverages **BioBERT** and **BERT** models for various **NLP tasks in the medical domain**, including **Named Entity Recognition (NER), Question Answering (QA), and Standard Operating Procedures (SOPs) processing**.

## Installation

To install the required dependencies, run:

```bash
pip install transformers datasets pandas torch

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

Models Used

1. BioBERT for Medical NER
Fine-tuned BioBERT for Named Entity Recognition (NER) in medical text.
Pretrained Model: ktrapeznikov/biobert_v1.1_pubmed_squad_v2
Colab Notebook


# Load a BioBERT model fine-tuned for question answering
tokenizer = AutoTokenizer.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")
model = AutoModelForQuestionAnswering.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")

https://colab.research.google.com/drive/1eAv28qdWw8rNBmRxA6B7R0RIMs0v7-Ht?usp=sharing


used model 

# Load BERT MODEL AND FINETUNE USING CSV FILE
BERT

fine tune give csv file it has only 10 data higher the dataset higher the accuracy . 

https://colab.research.google.com/drive/17JLaH6qkfFQespiHVgeS3blBJmXIa6tR?usp=sharing



# Load a BioBERT model fine-tuned for SOPS
used model in sops 

https://colab.research.google.com/drive/1IjqrqAgDR7h3CC6GpQwVZxaDgG8YjUjr?usp=sharing


tokenizer = AutoTokenizer.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")
model = AutoModelForQuestionAnswering.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")

Methodologies
1. Named Entity Recognition (NER)

Identifies medical entities such as diseases, symptoms, drugs, and procedures.

Utilizes a fine-tuned BioBERT model.

2. Question Answering (QA)

Uses BioBERT for medical question-answering.

Fine-tuned with medical QA datasets.

3. Fine-Tuning BERT for Medical Text Classification
BERT is trained on a CSV dataset.

A larger dataset improves classification performance.

4. Processing Standard Operating Procedures (SOPs)
Utilizes BioBERT to extract relevant information from medical SOPs.