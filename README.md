# Predictive-Model-for-delivery-orders
 #### Example:
 I am a vendor and one day I come up with a idea to add a new item called "Chicekn Fired Rice" to my menu. But I am not sure whether customer will like it or not. So, I can use this model to predict the orders. If the result is about 100 orders/month, I will feel confident about this idea. If the result shows only 10 orders/month, I will need to sleep on this and reconsider my choice. At the mean time, by the corelation chart here in the model, I will know which feature will mostly effect the orders, so I can act on this and make some changes to product name and description to gain more orders. 
    

**Solutions:**

1. Based on given data, build a **predictive model** to predict the possible sales/orders. So vendors can use this model to predict their sales/ orders based on the type of product and the description of the product.


**Steps:**
1. **Import Libs & Data**
2. **Data Exploration & Cleaning**
3. **Feature Engineering**

    3.1 How many product one vendor have (A rough measure of vendor size)
    
    3.2 What's the popularity of one vendor_geohash (# of vendor in one vendor_geohash)
    
    3.3 Wheather the product have a description or not (boolean)
    
    3.4 Length of the Product name & Length of the Product description
    
    3.5 Create new Features based on above NLP anlysis
    
        * How many popular key words the product name contains
        
        * How many popular key words the product description contains
        

4. **Build Predictive Models & Validation**
5. **Future improvements**

**Future Improvements**

1. **Put more time and effort to feature engineering & data cleaning.**


    1.1 Use geo location data to cluster data and for each cluster we can generate corresponding features. 
        For example:
        most popular product name keywords in certain area.
        
        
    1.2 NLP can be applied to measure the similarity of product_name and product_description. This can also be a 
        interesting feature to look at.
        
        
    1.3 Tag tokens with NLTK and calculate the distribution of tags for each name and description. 
    
    
    1.4 Use domain knowlegde further cluster data. For example, we can cluster product names to several 
        classes and use it as categorical data. Like: Rice, Noodle, Pizza, Soup, Drink, Main Dish....



2. **Tuning the model**.


    2.1 Cross-validtion
    
    2.2 Grid-search to tune parameters
    
    2.3 Try more models and build ensemble models.
    
    2.4 Try Lighgbm with categorical data to see the performance.

3. **Add test cases for help functions in the notebook**
