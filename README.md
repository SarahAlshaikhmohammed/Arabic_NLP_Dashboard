
# Arabic NLP Dashboard Project

This project consists of two main components:
1. **Arabic Speech to Text Conversion**: A Python script that processes Arabic audio files, splits them into manageable chunks based on silence, and transcribes the audio into text.
2. **Arabic Text Preprocessing**: A comprehensive text processing pipeline for Arabic, which includes removing punctuation, stopwords, normalizing text, tokenization, and generating word frequency and sentiment analysis.

## Project Overview

The processed data is visualized using **Power BI** to generate an interactive **Arabic NLP Dashboard** that provides insights into the transcribed and preprocessed text. This includes sentiment analysis, topic modeling, and named entity recognition (NER) results.

### Key Components:

- **Speech-to-Text Conversion**: Converts Arabic audio files into text using the `speech_recognition` library and Google Speech-to-Text API.
- **Text Preprocessing**: Includes punctuation removal, stopword removal, text normalization, and tokenization for Arabic text.
- **Sentiment Analysis**: Uses CAMeL Tools to predict the sentiment (positive, negative, or neutral) of Arabic sentences.
- **Topic Modeling**: Applies Latent Dirichlet Allocation (LDA) to group sentences into topics.
- **Named Entity Recognition (NER)**: Identifies and categorizes named entities (such as persons, organizations, and locations) in the Arabic text using CAMeL Tools.
- **Arabic NLP Dashboard**: Provides visual insights into word frequencies, sentiments, topics, and named entities using Power BI.

### Power BI Dashboard Preview:

![Arabic NLP Dashboard](/NLP_Dashboard.png)

The dashboard offers a detailed visual representation of key insights from the Arabic text data.

## How to Run

1. Clone or download the project repository.
2. Install the required Python libraries:
   ```bash
   pip install pydub pytube speechrecognition google-cloud-storage ffmpeg python-docx pyarabic qalsadi camel-tools
   ```
3. Mount Google Drive if working in Google Colab.
4. Run the provided scripts for Arabic Speech-to-Text conversion and Arabic Text Preprocessing.
5. Load the output files (`word_frequency.csv`, `sentiments.csv`, `topics.csv`, `entities.csv`) into Power BI to create the dashboard.

## How to Use

- Use the **Speech-to-Text Conversion** script to convert Arabic audio files into text.
- Apply the **Text Preprocessing** pipeline to clean and process the text.
- Visualize the processed data in **Power BI** to extract insights from the NLP analysis.

## Output Files

- `word_frequency.csv`: Contains word frequencies for the processed Arabic text.
- `sentiments.csv`: Contains sentiment analysis results for each sentence.
- `topics.csv`: Contains topic modeling results for each sentence.
- `entities.csv`: Contains named entities and their categories.

## License

This project is open-source and available under the MIT License.
