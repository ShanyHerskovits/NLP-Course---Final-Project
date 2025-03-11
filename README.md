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

3. **Training Combinations** (4 models total):
   - BERT trained on DreamBank
   - BERT trained on DREAM dataset
   - GPT-2 trained on DreamBank
   - GPT-2 trained on DREAM dataset

4. **Evaluation**: All four models were tested on the same test set of 50 dreams with interpretations

## Key Results

Your evaluation metrics (BLEU, ROUGE, BERTScore, perplexity) showed different strengths across the models:

1. **BERT + DreamBank**:
   - Template-based approach with regression output
   - Very low lexical matching (BLEU ~0.003)
   - High semantic understanding (BERTScore ~0.87)

2. **BERT + DREAM dataset**:
   - Classification approach for multiple-choice
   - Moderate classification accuracy
   - Different performance profile than DreamBank training

3. **GPT-2 + DreamBank**:
   - Generative approach with low lexical matching (BLEU ~0.006)
   - Good semantic understanding (BERTScore ~0.84)
   - Generated coherent interpretations

4. **GPT-2 + DREAM dataset**:
   - Multiple-choice selection approach
   - Higher accuracy (~48%) than random baseline
   - Different lexical metrics than generative approach

The project effectively demonstrates how different training data and model architectures lead to varying performance profiles for dream interpretation tasks, with interesting trade-offs between lexical precision and semantic understanding.
