# AI-Generated-Text-Detector










 This project was developed during the OpenData community hackathon for the Gitcoin GR15 Beta Round. 
   



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="Methodology">methodology</a></li>
     <li><a href="Conclusion">Conclusion</a></li>
     <li><a href="Suggestion">Suggestion</a></li>
  </ol>
</details>



## ABOUT THE PROJECT

Use of AI Generated Text has turend out to be one of the ways most cyber perpetrators common referred to as Sybils in ths context describe their projects during the appilcation phase. Also, Statistics shows that this traits has a probabilty of increasing over time. To mitigate this, I built project for the community to build upon in mitigating this challenge. During the GR15 Beta analysis, I tried searching for a similar open source projects to enable me build upon on Legos that I made use for my analysis but surprisingly I found non. This model though not yet perfect but a promising start for mitigating this problem of AI Generated Texts.

 
 ###  Model
 
The AI Text Detector model uses XGBoost, a powerful and popular machine learning algorithm, to analyze the text. XGBoost is a gradient boosting framework that has proven effective in natural language processing tasks such as text classification. The model has been trained on a large corpus of both human-written and AI-generated text to accurately identify specific features of text that are indicative of AI generation.

#### Project Implementation

The AI Text Detector project preprocesses the text by removing any unnecessary characters and converting it to a standardized format. The model then extracts specific features of the text such as repetitive patterns, unnatural phrasing, and an overuse of technical jargon, to determine whether the text was generated by AI. For future improvement, the model would also contain an ensemble approach later on, combining multiple machine learning models to increase the overall accuracy of the detection process after future updates. This approach would allow the model to more accurately detect AI-generated text while minimizing false positives.


 




<!-- GETTING STARTED -->
## Getting Started

To get started with this project, the installation of some python packages are required.

### Prerequisites

* numpy 
  ```sh
  pip install numpy 
  ```
  
* enchant
  ```sh
  pip install enchant
  ```
  
* sklearn
  ```sh
  pip install sklearn
  ```
  
* xgboost 
  ```sh
  pip install xgboost 
  ```
  
* nltk
  ```sh
  pip install nltk
  ```
  
* string
  ```sh
  pip install string
  ```
  
* pandas 
  ```sh
  pip install pandas 
  ```
  
* nltk
  ```sh
  pip install nltk
  ```



<!-- USAGE EXAMPLES -->
## Methodology

### Data Collection

The AI Text Detector project requires a large corpus of text data that includes both human-written and AI-generated text. GPT Wiki Intro dataset developed by Google hugging face was used for this project.
The [GPT Wiki Intro Dataset](https://huggingface.co/datasets/aadityaubhat/GPT-wiki-intro) contains Wikipedia introductions and GPT (Curie) generated introductions for 150k topics. To generate an AI generated text this prompt was used in ChatGPT.


* Prompt
  ```sh
  200 words wikipedia style introduction on '{title}'
  {starter_text}
  ```

where title is the title for the wikipedia page, and starter_text is the first seven words of the wikipedia introduction.

### Data Preprocessing

The text data underwent several preprocessing steps to ensure the quality of the data and the model training. I removed any unnecessary characters, such as punctuation marks, and converted the text to a standardized format. I also performed other standard preprocessing steps such as lowercasing, stemming, and lemmatization to ensure that the data is consistent and of high quality. 
   #### Feature Transformation

For the model training I had to create a new feature called Output. I acheived this by importing the text data as two seperate dataframe, transforming it then union both datasets. I also had to randomise the final training data model to avoid over fitting.

### Feature Extraction

I identified specific features of the text that are indicative of AI generation. These features include repetitive patterns, unnatural phrasing, punctuations, and an overuse of technical jargon. I also used various techniques such as statistical analysis and machine learning algorithms to identify these features accurately behind the background.

### Model Training

I used XGBoost, a powerful machine learning algorithm, to develop the AI Text Detector model. We trained the model using the preprocessed text data and the extracted features. We also employed an ensemble approach, combining multiple machine learning models to increase the overall accuracy of the detection process.

   


## Conclusion.

The AI Text Detector model uses advanced machine learning and natural language processing techniques to identify AI-generated text accurately. Preventing fraudulent grant projects on the Gitcoin Beta Round funding, this project helps to maintain the platform's integrity and ensure that only genuine projects receive funding.

## Suggestions

* The  model can be imporved by adding more parameters and tunning it more to improve the accuracy
* Extra features can be added to the model tp improve its performance
* More algorithms can be ensembled into the model to improve its prediction power.





