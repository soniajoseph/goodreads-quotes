![](assets/images/posts/goodreads.png)

Looking for material to run semantic searches on, I was surprised that I could not find a database of Goodreads quotes online. Kaggle has datasets for the [other kinds of Goodreads data](https://www.kaggle.com/jealousleopard/goodreadsbooks), but no quotes. The Goodreads API does not allow for quote scraping either.

This Python quote scraper gets the quote text, title, author, tags, and number of likes. If you enter the author name, with number of pages of quotes as an optional argument, the scraper will both print the results in the Terminal and return them as a list. If you don't specify a page number, the scraper will get quotes from all the pages available on Goodreads.

The command is:
```python
>>> quotes_by_author(author, page_num=None):
```

An example...
```python
>>> quotes_by_author("jk rowling")
looking through 6244 pages
scraping page 1
scraping page 2
...

...

```

Snippet of results...
```python
scraping page 1
“If you want to know what a man's like, take a good look at how he treats his inferiors, not his equals.”  
  ―
J.K. Rowling
Harry Potter and the Goblet of Fire
None
95138

“It is our choices, Harry, that show what we truly are, far more than our abilities.”
J.K. Rowling
Harry Potter and the Chamber of Secrets
['choices']
49192

“It does not do to dwell on dreams and forget to live.”
J.K. Rowling
Harry Potter and the Sorcerer's Stone
['life']
47176

“I solemnly swear that I am up to no good.”
J.K. Rowling
Harry Potter and the Prisoner of Azkaban
[]
37420
```

I fed a list of all the authors on Goodreads into the scraper to build a database of quotes, which I will release on Kaggle soon.