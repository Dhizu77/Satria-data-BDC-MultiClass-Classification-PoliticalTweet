
# Tweet Classification Using IndoBERT

This repository contains code for classifying a dataset of tweets into 8 distinct classes using a fine-tuned **IndoBERT** model. **The dataset is not provided due to its sensitive nature**, but instructions are included on how to use your own dataset with the model.

## Overview

The notebook performs the following tasks:

1. **Data Preparation**: Pre-processes and tokenizes tweets using the IndoBERT tokenizer.
2. **Model Training**: Fine-tunes a pre-trained IndoBERT model for tweet classification.
3. **Prediction**: Uses the trained model to classify tweets into 8 categories.

## Dataset

- The dataset used in this project is not included due to privacy concerns.
- To run the notebook, you need to provide your own dataset in CSV format with a column named `Text` that contains the tweets.

## Instructions

1. **Prepare your dataset**: Ensure your dataset has a structure similar to the following example:

   | Text                                   |
   |----------------------------------------|
   | "This is an example tweet."            |
   | "Another tweet example."               |

2. **Update the file path**: In the notebook, replace the placeholder `path/to/your/data.csv` with the actual path to your dataset file.

3. **Install necessary libraries**:
   ```bash
   pip install transformers torch pandas
   ```

4. **Run the notebook**: Load the notebook in a Jupyter environment or Google Colab, and execute each cell to process and classify your data.

## Model Details

- **Tokenizer**: IndoBERT tokenizer (`AutoTokenizer`)
- **Model**: IndoBERT for sequence classification (`AutoModelForSequenceClassification`)
