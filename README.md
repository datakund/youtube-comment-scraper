## Youtube-Comment-Scraper
A python library that uses browser automation to scrape youtube comments
It uses [datakund](https://pypi.org/project/datakund) internally

Complete Documentation available [here](https://youtube-api.datakund.com/en/latest/)


### Support
For any help / feedback you can message us here
* datakund@gmail.com
* https://t.me/datakund

### Installation

```sh
pip install youtube-comment-scraper
```

### Import

```javascript
from youtube-comment-scraper import *
```

### Open Video

To open video we use ``open`` function
It requires **url** as input parameter

```javascript
youtube.open("place_video_url_here")
```

### Scroll Down

To bring video comments into view we will scroll the page using ``keypress`` function
It requires **key** as input parameter
We will use **pagedown** key to scroll the page down

```javascript
youtube.keypress("pagedown")
```

### Fetch Comments

To fetch comments we use ``video_comments`` function
It does not require any input parameter
It will fetch comments of any youtube video opened in browser

```javascript
response=youtube.video_comments()
comments=response['body']
```

### Example Response

```sh
[
   {
      "Comment":"Comment",
      "UserLink":"UserLink",
      "user":"user",
      "Time":"Time",
      "Likes":"Likes"
   }
   ,{}
   ,..
]
```

### DataKund
It uses [datakund](https://pypi.org/project/datakund/) internally to do browser automation
DataKund is an automation library that uses selenium & supports automation of many sites including [Youtube](https://youtube-api.datakund.com/en/latest/), [Amazon](https://amazon-api.datakund.com/en/latest/), [Twitter](https://twitter-api.datakund.com/en/latest/), [LinkedIn](https://linkedin-api.datakund.com/en/latest/) , [Google](https://google-api.datakund.com/en/latest/) etc.
