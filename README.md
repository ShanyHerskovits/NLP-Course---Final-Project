# NLP-Course---Final-Project
Presenters: Shany Herskovits and Ofir Nahshon

## Project Structure

We worked with two distinct datasets and two model architectures, creating four different trained models:

1. **Datasets**:
   - **DreamBank dataset**: Collection of real dream reports with interpretations
   - **DREAM dataset**: Dialogue-based reading comprehension dataset with multiple-choice questions

2. **Models**:
   - **BERT-based models**: For classification/regression approaches
   - **GPT-2 models**: For generative/classification approaches
   - **Llama-3.1-8B**: For generative approach

3. **Training Combinations** (5 models total):
   - BERT trained on DreamBank
   - BERT trained on DREAM dataset
   - GPT-2 trained on DreamBank
   - GPT-2 trained on DREAM dataset
   - Llama-3.1-8B trained on DreamBank

4. **Evaluation**: All five models were tested on the same test set of 50 dreams with interpretations

## Key Results

Your evaluation metrics (BLEU, ROUGE, BERTScore, perplexity) showed different strengths across the models:

1. **BERT + DreamBank**:
   - Template-based approach with regression output
   - Very low lexical matching (BLEU ~0.003)
   - High semantic understanding (BERTScore ~0.87)

2. **BERT + DREAM dataset**:
   - Classification approach for multiple-choice
   - Low classification accuracy

3. **GPT-2 + DreamBank**:
   - Generative approach with low lexical matching (BLEU ~0.002)
   - Good semantic understanding (BERTScore ~0.81)

4. **GPT-2 + DREAM dataset**:
   - Multiple-choice selection approach
   - Higher accuracy (~68%) than random baseline (33%)

5. **Llama-3.1-8B + DreamBank**:
   - Generative approach with low lexical matching (BLEU ~0.004)
   - Good semantic understanding (BERTScore ~0.83)


The project effectively demonstrates how different training data and model architectures lead to varying performance profiles for dream interpretation tasks, with interesting trade-offs between lexical precision and semantic understanding.
