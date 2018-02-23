# MERCARI PRICE PREDICTION 


**This project was run on Kaggle competition** (https://www.kaggle.com/c/mercari-price-suggestion-challenge)

In this competition, Mercari(Japan’s biggest community-powered shopping app) challenging you to build an algorithm that automatically suggests the right product prices. You’ll be provided user-inputted text descriptions of their products, including details like product category name, brand name, and item condition.


Product pricing gets even harder at scale, considering just how many products are sold online. Clothing has strong seasonal pricing trends and is heavily influenced by brand names, while electronics have fluctuating prices based on product specs.





## Data fields

Dataset can be downloaded from this link [data](https://www.kaggle.com/c/mercari-price-suggestion-challenge/data)

**train.tsv, test.tsv**

The files consist of a list of product listings. These files are tab-delimited.

* train_id or test_id - the id of the listing
* name - the title of the listing. 
* item_condition_id - the condition of the items provided by the seller
* category_name - category of the listing
* brand_name
* price - the price that the item was sold for. This is the target variable that you will predict. The unit is USD. This column doesn't exist 
   in test.tsv since that is what you will predict.
* shipping - 1 if shipping fee is paid by seller and 0 by buyer
* item_description - the full description of the item. Note that we have cleaned the data to remove text that look like prices (e.g. $20) to   
  avoid leakage. These removed prices are represented as [rm]

