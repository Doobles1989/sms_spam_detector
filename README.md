# SMS Spam Detector

## Overview
The **SMS Spam Detector** is a machine learning application that classifies text messages as either "spam" or "not spam" (ham). This project uses a linear Support Vector Classification (SVC) model and is hosted using Gradio to provide a user-friendly interface for testing messages.

## Features
- **Machine Learning Model**: A linear SVC model trained to classify SMS messages.
- **Text Classification**: Identifies whether a text message is spam or ham.
- **User Interface**: A Gradio app for inputting messages and displaying classification results.

## Files
- `gradio_sms_text_classification.ipynb`: Jupyter notebook containing the Gradio interface and the SMS classification function.
- `sms_text_classification_solution.ipynb`: The solution notebook with the initial implementation of the text classification model.
- `SMSSpamCollection.csv`: Dataset used for training the model, containing labeled SMS messages.

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/sms_spam_detector.git
   cd sms_spam_detector
Install Dependencies:
bash
Copy code
pip install pandas scikit-learn gradio
Usage
Train the Model:

Open the gradio_sms_text_classification.ipynb notebook.
Execute the cells to train the model using the provided dataset.
Run the Gradio Interface:

Launch the Gradio app by running the notebook or the Python script containing the interface code.
Enter a text message into the input box and click "Submit" to see the prediction.
Example Text Messages for Testing

## Example Text Messages for Testing
Use the following messages to test the SMS Spam Detector:
- "You are a lucky winner of $5000!"
- "You won 2 free tickets to the Super Bowl."
- "You won 2 free tickets to the Super Bowl text us to claim your prize."
- "Thanks for registering. Text 4343 to receive free updates on medicare."

## Project Structure
- `gradio_sms_text_classification.ipynb`: Main notebook for running the app.
- `sms_text_classification_solution.ipynb`: Initial solution notebook.
- `SMSSpamCollection.csv`: CSV file containing the labeled dataset.

## Model Implementation
### Data Preparation
- Features are extracted from the `text` column of the dataset.
- Targets are extracted from the `label` column.
- Data is split into training (67%) and testing (33%) sets.

### Pipeline
- A pipeline is built using `TfidfVectorizer` for feature extraction and `LinearSVC` for classification.

### Training
- The model is trained on the training dataset and evaluated on the testing dataset.

## Gradio Interface
### Function
- Takes user input (text message) and returns the classification result.

### Interface
- Two text boxes are provided—one for input and one for the output result.

## Requirements
- Python 3.6 or later
- Libraries: `pandas`, `scikit-learn`, `gradio`

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
