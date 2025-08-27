# NLP Model Training and Evaluation

This project focuses on training and evaluating Natural Language Processing (NLP) models for sequence classification tasks. The models are fine-tuned on multiple datasets and evaluated using various metrics, including F1 scores and confusion matrices.

## Features

- **Dataset Handling**: Includes preprocessing, tokenization, and mapping of datasets.
- **Model Training**: Fine-tunes `roberta-large` models on general and subset-specific datasets.
- **Custom Trainer**: Implements a custom loss function for multi-label classification.
- **Evaluation**: Computes F1 scores and generates confusion matrices for model evaluation.
- **Validation**: Validates models using external files and Perl-based evaluation scripts.

## Project Structure

- **`NLP.ipynb`**: Jupyter Notebook containing the entire workflow, including data preprocessing, model training, evaluation, and validation.
- **Datasets**: The project uses datasets for tasks like sequence alignment and classification.
- **Google Drive Integration**: Models and datasets are stored and accessed via Google Drive.

## Requirements

The project requires the following dependencies:

- Python 3.8+
- PyTorch
- Transformers
- Datasets
- Evaluate
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

Install the required Python packages using the following commands:

```bash
pip install datasets==3.5.0
pip install pyarrow==20.0.0
pip install transformers evaluate accelerate
```

## Usage

1. **Setup Environment**: Ensure all dependencies are installed and the required datasets are available in the specified paths.
2. **Run Notebook**: Open `NLP.ipynb` and execute the cells sequentially.
3. **Train Models**: Fine-tune the models on the general dataset and subsets like `images`, `headlines`, and `answers-students`.
4. **Evaluate Models**: Evaluate the trained models using F1 scores and confusion matrices.

## Results

The project evaluates models on multiple datasets and provides insights into their performance through:

- F1 scores for classification tasks.
- Confusion matrices for detailed error analysis.