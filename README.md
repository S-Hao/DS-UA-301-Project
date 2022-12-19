# DS-UA-301-Project

This project was inspired by [a rather generic article](https://itechindia.co/us/blog/which-of-the-3-algorithms-models-should-you-choose-for-sentiment-analysis-2/) about various approaches to sentiment analysis. Despite being an article on sentiment analysis methodology, there was no code to be found, so I wanted to see how they stacked up to each other. 

For this project, I chose 2 datasets, one containing IMDb reviews of either positive or negative sentiment, and the other containing emails of either athiest or christian sentiment.

For the lexicon approach, found in 'Final_Project_Lexicon.ipynb', I used sentiwordnet to calculate a sentiment score for each text. For the ML approach, found in 'Final_Project_CNN.ipynb', I chose a simple CNN for classification; as per the findings of a [sample project](https://github.com/LW0214/301_project), the simplest cnn model performs just as well as more complicated models such as LeNet. For the hybrid approach, found in 'Final_Project_Hybrid.ipynb', I vectorized the text data and fit a SGDClassifier onto it. 

Lexicon results:<br>
The tagging and score assignment time on the 20newsgroups dataset is 53 seconds.<br>
The accuracy of a sentiwordnet mapping on the 20newsgroups dataset is 53.78%.<br>
The tagging and score assignment time on the IMDb dataset is 668 seconds, or 11 minutes and 8 seconds.<br>
The accuracy of a sentiwordnet mapping on the IMDb dataset is 61.35%.<br>

CNN results:<br>
The total training time on the 20newsgroups dataset is 368 seconds, or 6 minutes and 8 seconds.<br>
The accuracy of a simple CNN on the 20newsgroups dataset after 5 epochs is 97.22%.<br>
The total training time on the IMDb dataset is 2742 seconds, or 45 minutes and 42 seconds.<br>
The accuracy of a simple CNN on the IMDb dataset after 5 epochs is 85.13%.<br>

Hybrid results:<br>
The vectorization and training time on the 20newsgroups dataset is 0.497 seconds.<br>
The accuracy of a SGDClassifier on the 20newsgroups dataset is 93.31%.<br>
The vectorization and training time on the IMDb dataset is 8.953 seconds.<br>
The accuracy of a SGDClassifier on the IMDb dataset is 88.48%.<br>


The above results can also be found in their respective .ipynb file.


In the 'shap-visualizations' folder are several examples of shap visualizations, as they are not properly displayed in the .ipynb files.


Special thanks to: <br>
https://github.com/LW0214/301_project <br>
https://www.kaggle.com/code/yommnamohamed/sentiment-analysis-using-sentiwordnet/notebook#TF-IDF-model
