# Persian Text Categorization 
This project applies machine learning techniques to classify Persian text data into predefined categories, such as music, sports, health, and more. By leveraging Natural Language Processing (NLP) techniques, the model processes and categorizes content from Persian websites based on their textual content, including titles, descriptions, and other metadata.

## Dataset

### Dataset Description

This dataset contains Persian text data collected from the Yektanet platform. It includes articles from various domains, such as news, sports, music, and more. Each entry in the dataset contains the following columns:
**Note:** The dataset is proprietary, and thus, its publication is not permitted.


| Column            | Description                      |
|-------------------|----------------------------------|
| category          | The category or subject of the content (target variable). |
| description       | A brief description of the content. |
| text_content      | Full content of the article. |
| title             | The title of the article. |
| h1                | Content of the H1 HTML tag. |
| h2                | Content of the H2 HTML tag. |
| url               | The URL of the article. |
| domain            | The domain of the website. |
| id                | Unique identifier for each article. |

### Dataset Location
- **Data/**: This folder will contain the dataset files.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure

The main folders and files in the project are structured as follows:

```plaintext
Text-Categorization/
├── Data/
│   └── [dataset files will be here]
├── Notebook/
│   └── [your Jupyter notebooks will be here]
└── README.md
```

## Feature Engineering and Data Preprocessing
- The text data undergoes several preprocessing steps:
  - Removal of punctuation
  - Normalization of text (e.g., handling Persian characters)
  - Stemming
  - Tokenization and filtering of stopwords
  - TF-IDF vectorization for converting text to numerical features
- The dataset is balanced using oversampling techniques to address class imbalance.

## Model Training
- The project uses a Support Vector Machine (SVM) model with a linear kernel to perform text categorization.
- The training dataset is split into training and testing sets, and an oversampling technique (RandomOverSampler) is applied to balance the dataset.

## Model Performance
The model achieved the following F1 scores:
- **Training Set:** 0.9937
- **Test Set:** 0.7356

## Requirements
To run the project, you will need the following Python packages:

- `pandas`
- `sklearn`
- `imblearn`
- `re`
- `hazm` (for Persian NLP tasks)
