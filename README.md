# Sentiment Analysis on Tweets about Feminism


## Project Overview

Understanding public sentiment around feminism is crucial for detecting social trends, identifying potential misinformation, and analyzing the evolution of public discourse. 

This project classifies tweets mentioning feminism into five sentiment categories using a **pre-trained NLP model**.

## Key Features

- Uses the **nlptown/bert-base-multilingual-uncased-sentiment** pre-trained model.  
- Classifies tweets into **five sentiment categories**: *Very Negative, Negative, Neutral, Positive, Very Positive*.  
- **Data visualization** using bar charts.  
- **Bias detection & error analysis** for evaluating the model’s performance. 

## Why It Matters

Analyzing sentiment around feminism is not just a technical exercise — it helps to:
- **Detect polarization** and identify trending narratives around feminist topics.
- **Understand how public discourse evolves over time.**
- **Evaluate language model biases** when applied to sensitive topics. 

This project highlights the **importance of combining automated analysis with human review**, especially when dealing with **cultural nuances and ideological debates**.  

## Dataset

- **Source:** A collection of tweets using hashtags like `#feminismo`, `#8M`, `#igualdad`, etc.

## Technologies Used

- **Python 3.6+**
- **Transformers (Hugging Face)**
- **Pandas**
- **Matplotlib**

## Installation and Usage

### Local Execution

1. **Clone the repository**
   git clone https://github.com/BeaEsparcia/Sentiment_Analysis_on_X_Feminism.git
   cd Sentiment_Analysis_on_X_Feminism

2. **Install dependencies**
   pip install -r requirements.txt

3. **LaunchJupyter Notebook and open the notebook**
   Jupyter Notebook

4. **Run the notebook**
   Open Sentiment_Analysis_on_X_Feminism.ipynb and execute all cells.

### Local Execution
If you prefer to run the project on Google Colab, click the button below:
https://colab.research.google.com/github/BeaEsparcia/Sentiment_Analysis_on_X_Feminism/blob/main/Sentiment_Analysis_on_X_Feminism.ipynb

If necessary, install the required libraries at the beginning of the notebook:
!pip install transformers pandas matplotlib
   
## Methodology
### Text Preprocessing

- **Removal of emojis, links, and unnecessary symbols.**
- **Basic normalization** (lowercasing).

### Sentiment Classification

Each tweet was classified using **nlptown/bert-base-multilingual-uncased-sentiment**, a **multilingual sentiment analysis model.**

### Visualization

- Sentiment distribution was visualized using **bar charts.**
- **Manual review of incorrect classifications** to detect biases.

### Error Analysis & Bias Detection

**Findings**
- The model performed **well in neutral and straightforward cases.**
- It **struggled with contextual and cultural nuances**, leading to misclassifications.

**Examples of Incorrect Classifications**
- "YES. I AM A FEMINIST." → Labeled Very Negative → Possible bias.
- A tweet criticizing feminism → Labeled Very Positive.
 
## Limitations and areas for improvement

- **Fine-tuning the model:**: Training on a feminism-specific dataset would improve accuracy.
- **Heuristic rules:**: Adding keyword-based corrections could prevent obvious misclassifications.
- **Manual review phase**: Essential for identifying biases and refining results.
- **Expanding the dataset:**: A larger dataset would provide a more representative analysis.
- **Subjectivity analysis:**:  Distinguishing opinions vs. facts could enrich insights.
 
## What I Learned

- **Applying NLP to sensitive topics requires critical thinking beyond technical implementation.**
- **Cultural nuances matter** — Models trained on general sentiment data often fail in ideological debates.
- **Combining AI with human review** is **essential** for socially impactful NLP applications.
  
This project reinforced my interest in **ethical AI** and **responsible NLP**, especially in the context of **social justice topics.**

## Contributions

Contributions are welcome!
If you'd like to contribute, please open an issue first to discuss any proposed changes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact

Beatriz Esparcia
Email: esparcia.beatriz@gmail.com
LinkedIn: linkedin.com/in/beaesparcia
Project Link: GitHub Repository
