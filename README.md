# NLP-Medical-System

pip install transformers datasets pandas torch


used model in NER FOR MEDICAL

# Load a BioBERT model fine-tuned for question answering
tokenizer = AutoTokenizer.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")
model = AutoModelForQuestionAnswering.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")

https://colab.research.google.com/drive/1eAv28qdWw8rNBmRxA6B7R0RIMs0v7-Ht?usp=sharing

used model 
# Load BERT MODEL AND FINETUNE USING CSV FILE
BERT

fine tune give csv file it has only 10 data higher the dataset higher the accuracy . 

https://colab.research.google.com/drive/17JLaH6qkfFQespiHVgeS3blBJmXIa6tR?usp=sharing


used model in sops 

https://colab.research.google.com/drive/1IjqrqAgDR7h3CC6GpQwVZxaDgG8YjUjr?usp=sharing

# Load a BioBERT model fine-tuned for SOPS
tokenizer = AutoTokenizer.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")
model = AutoModelForQuestionAnswering.from_pretrained("ktrapeznikov/biobert_v1.1_pubmed_squad_v2")