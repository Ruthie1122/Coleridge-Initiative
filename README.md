Task
The goal of this project is to automate the discovery of datasets mentioned in scientific publications using Natural Language Processing (NLP) techniques. The challenge arises due to the diverse and unstructured ways datasets are referenced in research articles, making it difficult to identify them through traditional keyword searches. This project aims to streamline this process, making datasets easier to find, categorize, and access for researchers, data scientists, and policy analysts.

Description
This solution employs a variety of deep learning models like BiLSTM (Bidirectional Long Short-Term Memory), GRU (Gated Recurrent Units), and sep-CNN (Separately Convolutional Neural Network) to capture context and detect dataset mentions in scientific texts. Each model was trained and fine-tuned using labeled datasets provided in the Coleridge Initiative competition. Key features include:

Text Preprocessing: Tokenization, stopword removal, and word embedding to standardize input data.
Model Architecture: A hybrid approach using recurrent and convolutional layers to handle both sequential dependencies and local text patterns.
Ensemble Model: A final ensemble model combining predictions from BiLSTM, GRU, and sep-CNN for improved accuracy and robustness.
The models were evaluated using metrics like precision, recall, and F1-score, achieving high accuracy across diverse research fields.
Installation
To install and run the project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone <repository-url>  
cd Coleridge-Initiative  
Create and activate a virtual environment (optional but recommended):

bash
Copy code
python -m venv env  
source env/bin/activate  # On Windows use `env\Scripts\activate`  
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt  
Download or link the dataset (if required) and place it in the appropriate directory.

Usage
The project can be executed using the following command:

Train the models using the prepared dataset:

bash
Copy code
python train_models.py  
Test the models on the test dataset:

bash
Copy code
python evaluate_models.py  
Make predictions on new scientific publications:

bash
Copy code
python predict.py --input <path-to-new-document>  
View the results to see detected dataset mentions, annotations, and classifications.
