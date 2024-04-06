# USDA Prompt Matching using Fuzzy Matching and TF-IDF

This project demonstrates the process of matching USDA prompts with corresponding descriptions using fuzzy matching and TF-IDF vectorization techniques.

## Introduction

The USDA (United States Department of Agriculture) prompts are short textual descriptions, and they need to be matched with corresponding longer descriptions ('Descrip EN') for further analysis. This task is accomplished using fuzzy matching to find approximate matches and TF-IDF vectorization to represent text data numerically.

## Requirements

- Python 3.x
- Required Python libraries: `fuzzywuzzy`, `pandas`, `scikit-learn`

## Usage

1. Install the required Python libraries if not already installed:
   ```bash
   pip install fuzzywuzzy pandas scikit-learn
   ```

2. Run the provided Python script.

## Script Overview

1. **Data Loading**: The script loads data from an Excel file containing USDA prompts and corresponding descriptions.

2. **Preprocessing**: Text preprocessing is performed on both USDA prompts and descriptions. This includes converting text to lowercase, removing punctuation, and stripping whitespace.

3. **TF-IDF Vectorization**: TF-IDF (Term Frequency-Inverse Document Frequency) vectorization is applied to convert text data into numerical vectors.

4. **Fuzzy Matching**: Fuzzy matching is used to find approximate matches between USDA prompts and descriptions based on cosine similarity scores calculated using TF-IDF vectors.

5. **Result Visualization**: The matched USDA prompts and their corresponding descriptions along with similarity scores are presented in a DataFrame.

## Additional Notes

- The script assumes that the data is stored in an Excel file named 'LAST REVIEW.xlsx' and contains columns named 'usda prompt' and 'Descrip EN'. You may need to modify the script if your data is stored differently.
- Make sure to adjust file paths and column names accordingly if you're using a different dataset.

## References

- [FuzzyWuzzy Documentation](https://github.com/seatgeek/fuzzywuzzy)
- [scikit-learn Documentation](https://scikit-learn.org/stable/)

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to customize this README according to your preferences or add any additional information that you think would be relevant for users of your code.
