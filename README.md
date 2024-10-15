# Leveraging Machine Learning to Combat Fake News: A Multi-Classifier Approach for Social Media News Verification

## Project Overview
In the digital age, fake news has become a serious problem, influencing public opinion and decision-making. This project aims to combat fake news using machine learning to build models capable of detecting misinformation in news articles. The project focuses on the BuzzFeed dataset from FakeNewsNet, which contains both real and fake news articles.

## Motivation
The motivation for this project stems from the detrimental effects fake news can have on society, such as eroding trust in institutions and fueling societal division. Having personally witnessed the impact of fake news, especially during the pandemic, I wanted to contribute to the fight against misinformation by developing robust machine learning models that can help identify and flag fake news.

## Dataset
The dataset used for this project is the BuzzFeed News dataset from FakeNewsNet. This dataset includes news articles shared by nine news agencies during the 2016 U.S. election. The dataset is fact-checked by BuzzFeed journalists and consists of 91 articles with 12 features. It contains both real and fake news, making it suitable for training machine learning models to detect fake news.

## Exploratory Data Analysis (EDA) Insights
During the EDA phase, several interesting patterns were identified:
- **Thematic Priorities**: Fake news often highlights political figures like "Hillary" and "Clinton," whereas real news articles focus on broader topics, such as "Trump" and "debate."
- **Sensationalism**: Fake news titles frequently use sensational or biased language, with terms like "Muslim" and "terrorist" appearing more often.
- **Title Length**: Fake news tends to have slightly longer, attention-grabbing titles, while real news headlines are more concise.

## Machine Learning Models
The project employed several machine learning algorithms to classify fake and real news articles based on the body, titles, and a combination of both. The performance of the classifiers was evaluated using metrics like accuracy, precision, recall, and F1-score.

### Classification Performance
1. **Using News Body**:
   - **SVM**: 81% accuracy (F1-score: 80%)
   - **Naive Bayes**: 73% accuracy (F1-score: 71%)
   - **Random Forest**: 78% accuracy (F1-score: 78%)
   
2. **Using News Titles**:
   - **Naive Bayes**: 65% accuracy (F1-score: 70%)
   - **SVM**: 54% accuracy
   - **Random Forest**: 62% accuracy

3. **Using Both Titles and Body**:
   - **SVM**: 81% accuracy (F1-score: 79%)
   - **Naive Bayes**: 73% accuracy (F1-score: 71%)
   - **Random Forest**: 78% accuracy (F1-score: 78%)

The results highlight that combining both the body and title improves the model's accuracy in detecting fake news.

## Challenges and Limitations
Some of the challenges faced during the project included:
- **Preprocessing Text Data**: Converting raw text into meaningful features.
- **Feature Selection**: Choosing the most relevant features for model training.
- **Data Imbalance**: Managing imbalances in the dataset where certain types of news were underrepresented.

## Future Directions
Several areas of improvement and further research include:
- **Advanced Classification**: Exploring deep learning models for better accuracy.
- **Multimodal Analysis**: Incorporating metadata or social media metrics to enhance the model's understanding of news articles.
- **Real-time Detection**: Implementing the models for real-time monitoring of news feeds to quickly detect and flag misinformation.

## Ethical Considerations
While machine learning is a powerful tool to detect fake news, it’s important to address ethical concerns such as the potential for censorship and the need for transparency in algorithmic decision-making. The models should be designed to respect freedom of speech while ensuring fairness and accountability.

## How to Run the Project
- The code is available in the Jupyter notebook in this repository.
- The dataset folder contains the BuzzFeed dataset used for training and testing.
- The project report provides detailed insights into the model-building process and results.

## Repository Structure
- `/dataset/` – Contains the dataset
- `/report.pdf` – Project report
- `/code.ipynb` – Jupyter notebook with the code
- `/README.md` – This file

## Conclusion
This project demonstrates how machine learning can be leveraged to combat the spread of fake news, offering insights into the challenges and future potential of automated misinformation detection.

