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

* Place `products_export_1-2000.csv` file into `input` folder.
* Customize `input/google_category_mapping.csv` if required.
* Change `company` variable from "Example" to your company name.
* Execute Jupyter notebook
* Find converted file in `output/google_merchant.csv`

## Known bugs and TODOs

* Calculate `sale_price` based on promotion field `Promotion Discount`
* Review culculation of `availability` field (out of stock vs in stock)
* Remove unused columns

## Images link examples

* Thumbnail: https://www.example.co.nz/site/example/images//thumb/021.1106_RUPES-Filter-for-KS260.jpg
* Normal: https://www.example.co.nz/site/example/images/items/021.1106_RUPES-Filter-for-KS260.1.jpg
* Medium/Large: https://www.example.co.nz/site/example/images//large/021.1106_RUPES-Filter-for-KS260.jpg
* Large: https://www.example.co.nz/ic/example/3456745154/021.1106_RUPES-Filter-for-KS260.jpg