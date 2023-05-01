# merchant-export

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/thlaegler/merchant-export/HEAD?labpath=notebook.ipynb)

Jupyter notbook and pyhton program to convert Zest product CSV export file into [Google merchant product specification CSV file](https://support.google.com/merchants/topic/6324338) and [Facebook product catalogue specification CSV file](https://www.facebook.com/business/help/120325381656392).

## Getting started / TL;DR

### Execute Jupyter notebook locally

Requires python and pip.

```
$ git clone git@github.com:thlaegler/merchant-export.git
$ cd merchant-export
$ pip install --upgrade pip
$ pip install --upgrade ipython jupyter jupyterlab notebook pandas
$ jupyter notebook list
$ jupyter notebook
```

### Execute Jupyter notebook via MyBinder

Open Jupyter notebook in [My Binder](https://mybinder.org/v2/gh/thlaegler/merchant-export/HEAD?labpath=notebook.ipynb).

## Usage

* Copy `products_export_1-2000.csv` and `products_export_2001-4000.csv` file into [input](input) folder.
* Copy `google_category_mapping.example.csv` in [input](input) folder to `google_category_mapping.csv` and customize the category mapping according to your needs.
* Change `company` variable in Jupyter notebook from `Example` to your company name.
* Execute Jupyter notebook
* Find converted files `products_google.csv` and `products_facebook.csv` in [output](output) folder.

## Known bugs and TODOs

* Review calculation of `availability` field (out of stock vs. in stock). There are products in stock but the other column says out of stock in the source files?
* Remove unused columns
* Source files have products with price of 0.00 NZD?
* Promotion start date and end date is (almost) always the same?
* Source files have no active promotion date and some invalid promotion dates (e.g. 2022/11/31)

## Images link examples

* Thumbnail: https://www.example.co.nz/site/example/images//thumb/021.1106_RUPES-Filter-for-KS260.jpg
* Normal: https://www.example.co.nz/site/example/images/items/021.1106_RUPES-Filter-for-KS260.1.jpg
* Medium/Large: https://www.example.co.nz/site/example/images//large/021.1106_RUPES-Filter-for-KS260.jpg
* Large: https://www.example.co.nz/ic/example/3456745154/021.1106_RUPES-Filter-for-KS260.jpg