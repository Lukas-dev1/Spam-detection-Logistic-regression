
# Spam Detection using Logistic Regression

This project aims to build a spam detection model using Logistic Regression. The dataset contains SMS messages labeled as either 'ham' (not spam) or 'spam'. The goal is to accurately classify messages as either spam or not spam based on their content.

## Installation

To run the notebook, you will need to install the required libraries. The main dependencies for this project are:

- `wordcloud`
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

You can install these packages using the following command:

```bash
pip install wordcloud pandas numpy matplotlib scikit-learn
```

## Overview of the Notebook

1. **Data Loading**: The dataset containing SMS messages is loaded into a pandas DataFrame.
2. **Data Preprocessing**: 
   - The 'Category' column is converted into binary labels where 'ham' is encoded as 0 and 'spam' is encoded as 1.
   - Additional data preprocessing may include removing null values and cleaning text data.
3. **Visualization**: The word cloud library is used to visualize the most frequent words in spam and ham messages.
4. **Model Building**: 
   - Logistic Regression is used to build the spam detection model.
   - The dataset is split into training and testing sets.
   - The model's performance is evaluated using accuracy, precision, recall, and F1 score.
5. **Prediction**: The trained model is used to predict whether a message is spam or not.

## How to Use

- Clone this repository and navigate to the directory containing the notebook.
- Install the necessary packages using the provided installation command.
- Open the notebook and execute the cells to preprocess the data, train the model, and make predictions.

## Dataset Information

The dataset includes the following columns:

- **Category**: Indicates whether the message is spam or not ('ham' for non-spam and 'spam' for spam).
- **Message**: The content of the SMS message.

## Example Code Snippet

Here's an example of how the dataset is preprocessed:

```python
# Convert 'ham' to 0 and 'spam' to 1
df['Category'] = df['Category'].map({'ham': 0, 'spam': 1})
```

## License

This project is for educational purposes. Please refer to the original dataset's license for more details.
