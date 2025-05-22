# Spam Email Detection

This project implements a machine learning model to detect spam emails using the Spam Email Dataset. The model uses Logistic Regression with TF-IDF vectorization to classify emails as spam or non-spam.

## Dataset Information

The dataset used in this project contains:
- A collection of emails labeled as spam or non-spam (ham)
- Text content of emails
- Binary classification labels (spam/ham)
- Total of 5,728 email samples
- Balanced distribution between spam and non-spam emails

## Project Structure

```
spam_email_detection/
├── README.md
├── mail_detection.ipynb    # Jupyter notebook containing the implementation
└── data/                  # Directory containing the dataset
    └── emails.csv         # Dataset file
```

## Features

- Email spam detection using machine learning
- TF-IDF vectorization for text feature extraction
- Logistic Regression classifier
- Interactive command-line interface for checking emails
- Model evaluation metrics (accuracy score)
- Real-time email classification
- Support for batch processing of multiple emails

## Model Performance

The model achieves:
- Training accuracy: 99.65%
- Test accuracy: 98.34%

### Example Classifications

The model can accurately identify various types of spam emails:

1. Marketing Spam:
```
"Congratulations! You've won a million dollars. Just send us your credit card details to claim your prize."
[Classification: SPAM]
```

2. Phishing Attempts:
```
"Your account has been compromised. Please enter your personal information to secure it."
[Classification: SPAM]
```

3. Business Promotion:
```
"Increase your business revenue by 500% with our revolutionary new product. Click on a link to learn more."
[Classification: SPAM]
```

4. Legitimate Emails:
```
"Meeting scheduled for tomorrow at 2 PM in the conference room."
[Classification: NOT SPAM]
```

## Implementation Details

The spam detection model uses:
- TF-IDF Vectorization for text feature extraction
- Logistic Regression for classification
- 80-20 train-test split
- English stop words removal
- Text preprocessing (lowercase conversion)

### Technical Details

1. Data Preprocessing:
   - Text cleaning and normalization
   - Removal of special characters
   - Conversion to lowercase
   - Stop words removal

2. Feature Extraction:
   - TF-IDF vectorization
   - Minimum document frequency: 1
   - English stop words removal
   - Case-insensitive processing

3. Model Training:
   - Logistic Regression classifier
   - Binary classification (spam/not spam)
   - Cross-validation for model evaluation

## Usage

1. Clone this repository:
```bash
git clone https://github.com/Tamanna5/spam_email_detection.git
cd spam_email_detection
```

2. Install required packages:
```bash
pip install numpy pandas scikit-learn jupyter
```

3. Open and run the Jupyter notebook:
```bash
jupyter notebook mail_detection.ipynb
```

4. Use the interactive spam checker:
```python
# Example usage
input_mail = ["Your email text here"]
# The model will classify it as spam (1) or not spam (0)
```

### Interactive Mode

The notebook includes an interactive mode where you can:
- Check multiple emails in sequence
- Get immediate classification results
- Test different types of email content
- Evaluate model performance on custom examples

## Requirements

Key dependencies:
- Python 3.8+
- numpy
- pandas
- scikit-learn
- jupyter

## Potential Use Cases

1. Email Filtering:
   - Integration with email clients
   - Automated spam filtering
   - Custom spam detection rules

2. Security Applications:
   - Phishing detection
   - Malicious content identification
   - Security threat analysis

3. Business Applications:
   - Customer support email filtering
   - Marketing campaign analysis
   - Communication monitoring

## Future Improvements

Potential enhancements for the project:
1. Support for multiple languages
2. Integration with email APIs
3. Real-time learning from user feedback
4. Enhanced feature extraction methods
5. Support for attachment analysis
6. Web interface for easier interaction

## License

This project is licensed under the MIT License.

## Author

- [Tamanna5](https://github.com/Tamanna5)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change. 