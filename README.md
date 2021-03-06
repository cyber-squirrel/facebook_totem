# Totem
<a href="https://www.buymeacoffee.com/megadose" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
### Educational purposes only, if you have any suggestions, please do not hesitate to contact us.

Totem allows you to retrieve information about ads of a facebook page , we can retrieve the number of people targeted, how much the ad cost and a lot of other information. 

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
## Project example : [Totem maltego](https://github.com/megadose/totem-maltego)

# Demo
![HD Demo](https://github.com/megadose/gif-demo/raw/master/demo.mp4)
![](https://github.com/megadose/gif-demo/raw/master/demo.gif)

## ![hammer_and_wrench](https://github.githubassets.com/images/icons/emoji/unicode/1f6e0.png) Installation

### With PyPI

```bash
pip3 install facebook_totem
```

### With Github

```bash
git clone https://github.com/megadose/facebook_totem.git
cd facebook_totem/
python3 setup.py install
```

# Usage of Totem.py 

python3 Totem.py [-h] --mode MODE [--url URL] [--urls URLS] [--columns COLUMNS]
                [--target TARGET] --output OUTPUT

  -h, --help         show the help message and exit  
  --mode MODE There are different modes:  
  

​                              \- single : to get all ads on a page  

​                             \- multi : to get the ads on different pages  

​                             \- search : to search a page  

  --url URL          The url of the target page (single mode)  
  --urls URLS        Csv file with the lists of the target urls (multi mode)  
  --columns COLUMNS  The name of the column with the urls (multi mode)  
  --target TARGET    Target name (search mode)  
  --output OUTPUT    Name of the csv output file ( single and search mode )  

The output  is in the output folder, for the multi mode the name of the file is the name of the page + id of the page.  

# Usage of facebook_totem with python:

```python
from facebook_totem import *
getIdFromUrl(url) #to get a ID of a facebook page from the url of this page the output is the id
getFacebookPageFromName(name) #to search facebook page with a name the output is a list of the pages with this name
getAdsFromId(id) #to get all ads of a facebook page from the id of this page the output is a list of all ads
```

