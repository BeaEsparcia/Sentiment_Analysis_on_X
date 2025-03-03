# Sentiment Analysis on Tweets about Feminism


## Project Overview

Understanding public sentiment around feminism is crucial to detect social trends, identify potential misinformation, and analyze the evolution of public discourse. This project analyzes tweets mentioning feminism to classify their sentiment into five categories, using a pre-trained sentiment analysis model.

## Key Features

- Pre-trained model nlptown/bert-base-multilingual-uncased-sentiment. 
- Classification into 5 sentiment categories: very negative, negative, neutral, positive, very positive.
- Visualization of sentiment distribution using bar charts.
- Critical review of results and bias detection.

## Why It Matters

Analyzing sentiment around feminism is not just a technical exercise — it helps to:
- Detect polarization and identify trending narratives around feminist topics.
- Understand how public discourse evolves over time.
- Evaluate how well language models perform when applied to sensitive and politically charged topics.

This project also highlights the importance of combining automatic analysis with human review, especially when dealing with cultural nuances and ideological debates

## Dataset

- Source: Collection of tweets using hashtags like #feminismo, #8M, #igualdad, etc.

## Technologies Used

- Python 3.6+
- Transformers (Hugging Face)
- Pandas
- Matplotlib

## Installation and Usage

### Local Execution

1. Clone the repository:git clone https://github.com/tu-usuario/analisis-sentimientos-feminismo.git
cd analisis-sentimientos-feminismo
2. Install dependencies:pip install -r requirements.txt
3. Launch Jupyter Notebook and open
4. Launch Jupyter Notebook and open Analisis_Sentimientos_X.ipynb 
5. Set runtime type to GPU:
   - Go to "Runtime" > "Change runtime type"
   - Select "GPU"
6. Run all cells in order.

If you use Google Colab, you may need to install some libraries at the beginning of the notebook:
!pip install transformers pandas matplotlib

## Methodology
### Text Preprocessing

- Removal of emojis, links, and unnecessary symbols.
- Basic normalization (lowercase conversion).

### Sentiment Classification

- Each tweet was classified into one of 5 sentiment categories using nlptown/bert-base-multilingual-uncased-sentiment, a multilingual sentiment analysis model.

### Visualization

- Sentiment distribution was visualized using bar charts.
- Examples of incorrect classifications were reviewed and documented.

### Error Analysis & Bias Detection

- Manual review of misclassified tweets to identify bias or contextual misunderstanding.
- 
## Results

- The model performed reasonably well in neutral and clear-cut cases.
- However, it struggled with contextual and cultural nuances, leading to several incorrect classifications.
- Examples:
  - A tweet saying "SÍ. SOY FEMINISTA." was labeled as Very Negative, showing potential bias in the pre-trained model.
  - Another tweet criticizing feminism was labeled as Very Positive.
 
## Limitations and areas for improvement

- **Fine-tuning the model:**: Training the model on a feminism-specific dataset could significantly improve classification accuracy.
- **Heuristic rules:**: Adding simple keyword or phrase-based rules could automatically correct obvious misclassifications.
- **Manual review phase**: Including a manual review step would help catch clear errors and improve overall quality.
- **Expanding the dataset:**: Analyzing a larger and more diverse set of tweets would provide a more complete and representative picture.
- **Subjectivity analysis:**: i Adding a second layer of analysis to distinguish between subjective opinions and objective facts could enrich the insights.
 
## What I Learned

- Applying NLP to sensitive topics demands critical thinking beyond technical implementation.
- Cultural nuances matter — models trained on general sentiment data might fail in ideological debates.
- Combining automated analysis with human review is essential when dealing with social issues.
- This project reinforced my interest in ethical AI and responsible NLP, especially in the context of social justice topics.

## Contributions

Contributions are welcome. Please open an issue first to discuss any changes you'd like to propose.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact

Beatriz Esparcia - esparcia.beatriz@gmail.com
LinkedIn: www.linkedin.com/in/beaesparcia
Project Link: https://github.com/tu-usuario/analisis-sentimientos-feminismo
