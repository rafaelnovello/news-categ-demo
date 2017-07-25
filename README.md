# News Caterorizer Demo

It's a logistic regression demo showed first time at my personal blog linked in description area.

Basically, it's a python program for command line that download and process some news content from brasilian sites and use scikit-learn Logistic Regression to classify them in some categories.

# Install

- Clone the repo

- Install requirements (I'm guessing you are using virtualenv):
```
$ pip install -r requirements.txt
```

- Test instalation (It will show some help info)
```
$ python news_categorizer.py -h
```

# Use it

- You need to download and process the news data:
```
$ python news_categorizer.py -f links.csv -t base.pkl
```

  - I'm providing you the file with several news links, but you can make yours!

  - When it finish you'll see something like that:
  > Accuracy with 20% of testing data: 75%

- Now you could classify some news links like that:
```
$ python news_categorizer.py -t base.pkl -p <link>
```
