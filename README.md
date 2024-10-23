# Date Format Conversion Using Transformers

### Overview
This project implements a Transformer-based model using Hugging Face's T5 to convert dates from one format to another. Specifically, the model takes a date string in the format dd-mm-yyyy (e.g., "14-03-2020") and converts it into a natural language format (e.g., "The 14th of March 2020"). Sequence-to-sequence learning is used for this task using a pre-trained Transformer model.

### Dataset
The dataset consists of pairs of dates:
- Input Format: dd-mm-yyyy (e.g., "14-04-1990")
- Target Format: A natural language representation of the date (e.g., "14th of April 1990")

### Model Architecture
The model is based on the T5 Transformer architecture:
- Model Checkpoint: t5-small from Hugging Face.
- The model is fine-tuned to convert the input date string into the target format.
- Sequence-to-sequence learning is employed using Seq2SeqTrainer.

