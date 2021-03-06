# Indian Political Sentiments

An application that let the users search across all tweets related to the Indian political scenario through an input text phrase. 

By using the [Dash](https://plot.ly/products/dash/) framework, two graphs are presented --- a line chart for the sentiment across time, and a donut chart that aggregates the total sentiment. The data is obtained through a [tool](https://github.com/Jefferson-Henrique/GetOldTweets-python) to fetch old tweets while bypassing some Twitter API limitations. 
Sentiment is computed through [vaderSentiment](https://github.com/cjhutto/vaderSentiment), which is particularly well suited for social media text analysis. 

The app is deployed on Heroku and can be accessed on the following link (the dyno could be sleeping, please give it a minute to warm up!):
https://beautiful-olympic-21495.herokuapp.com/


## Wanna tinker?

- Install anaconda distribution for your OS and activate a virtual environment with Python version 3.6
```
conda create -n yourenvname python=3.6 anaconda
```
- Clone the GitHub repository
```
git clone https://github.com/rohitgupta91/polity_senti.git
```
- Install package requirements listed in requirements.txt
```
pip install -r requirements.txt
```
- Launch the application!
```
python app.py
```

---
References:
- https://github.com/timothyrenner/bigfoot-dash-app
- http://t-redactyl.io/blog/2017/04/using-vader-to-handle-sentiment-analysis-with-social-media-text.html
- https://github.com/datademofun/heroku-basic-flask
