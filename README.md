# merchant-export

Jupyter notbook and pyhton program to convert Zest product CSV export file into [Google merchant product specification CSV file](https://support.google.com/merchants/topic/6324338) and [Facebook product catalogue specification CSV file](https://www.facebook.com/business/help/120325381656392).

## Getting started / TL;DR

Run Jupyter notebook locally; requires python and pip.
```
$ pip install --upgrade pip
$ pip install --upgrade ipython jupyter jupyterlab notebook pandas
$ jupyter notebook list
$ jupyter notebook
```

## Usage

* Place `products_export_1-2000.csv` file into `input` folder.
* Customize `input/google_category_mapping.csv` if required.
* Execute Jupyter notebook
* Find converted file in `output/google_merchant.csv`

## Known bugs and TODOs

* Calculate `sale_price` based on promotion field `Promotion Discount`
* Review culculation of `availability` field (out of stock vs in stock)
* Remove unused columns

## Images links examples
* Thumbnail: https://www.wyatt.co.nz/site/wyatt/images//thumb/021.1106_RUPES-Filter-for-KS260.jpg
* Normal: https://www.wyatt.co.nz/site/wyatt/images/items/021.1106_RUPES-Filter-for-KS260.1.jpg
* Medium/Large: https://www.wyatt.co.nz/site/wyatt/images//large/021.1106_RUPES-Filter-for-KS260.jpg
* Large: https://www.wyatt.co.nz/ic/wyatt/3456745154/021.1106_RUPES-Filter-for-KS260.jpg