![](assets/images/posts/goodreads.png)

Looking for material to run semantic searches on, I was surprised that I could not find a database of Goodreads quotes online. Kaggle has datasets for the [other kinds of Goodreads data](https://www.kaggle.com/jealousleopard/goodreadsbooks), but no quotes. The Goodreads API does not allow for quote scraping either.

Thus I wrote a Python quote scraper which you can find on GitHub [here](), which gets the title, author, tags, and quote content. If you enter the author name, with number of pages of quotes as an optional argument, the scraper will return the quotes from the author in the Terminal.

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
```

I fed a list of all the authors on Goodreads into the scraper to build a database of quotes, which I will release on Kaggle soon.