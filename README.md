# Sentiment Analysis Project

This project is a sentiment analysis pipeline that takes textual feedback, processes it, performs sentiment analysis, and visualizes the results. The project supports integration with a MongoDB database for data storage and uses Flask for web-based interaction.

---

## Features

- **Random Data Generation**: Generate random textual feedback and insert it into a MongoDB database.
- **Data Preprocessing**: Clean and prepare the text data for analysis.
- **Sentiment Analysis**: Analyze the sentiment of the feedback using NLP techniques.
- **Visualization**: Create visual representations of the sentiment analysis results.
- **Web Interface**: A Flask-based web app for running the pipeline interactively.

---

## Project Structure

```plaintext
├── app.py                # Flask app for the web interface
├── main.py               # CLI script for the end-to-end pipeline
├── requirements.txt      # Python dependencies
├── setup.py              # Script for setting up project structure
├── config/               # Configuration files
│   └── db_config.py      # MongoDB configuration
├── data/                 # Directory for raw, processed, and log data
│   ├── raw/              # Raw data storage
│   ├── processed/        # Processed data storage
│   └── logs/             # Logs directory
├── models/               # Trained models (if applicable)
├── notebooks/            # Jupyter notebooks for exploration
├── outputs/              # Outputs directory
│   ├── graphs/           # Visualization outputs
│   └── reports/          # Analysis reports
├── src/                  # Core scripts for the pipeline
│   ├── data_generation.py   # Data generation script
│   ├── preprocess.py        # Data preprocessing script
│   ├── analysis.py          # Sentiment analysis script
│   └── visualization.py     # Visualization script
└── tests/                # Unit tests

```

## Installation

1. **Clone the Repository**
   ```
   git clone https://github.com/your-username/sentiment-analysis.git
   cd sentiment-analysis
   ```
2. **Set Up Virtual Environment**
```
  python -m venv venv
  source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. **Install Dependencies**
   ```
   pip install -r requirements.txt
   ```
   
4. **Set Up Project Structure**
   ```
   python setup.py
   ```
5. **Configure MongoDB**
   - Ensure MongoDB is running locally.
   - Update the `MONGO_URI` in `config/db_config.py` if needed.

---

## Usage

### Command Line Interface

Run the complete pipeline:
```
python main.py

### Web Application

Start the Flask app:
```
python app.py

Access the app at http://127.0.0.1:5000/
Use the following routes:
/generate: Generate random data.
/preprocess: Preprocess data.
/analyze: Perform sentiment analysis.
/visualize: Generate visualizations.







