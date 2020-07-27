# Forecast-for-all-products-paints-in-single-code

I worked on Paints Dataset. I have different Regions,Channels,Items,colours,sizes and my task is to forecast sales for 3 months for each size present in all products in specific Region and channel.

I used CNN-LSTM to train the model where my input data is present in Elastic search and forecasted results has to be pushed to MySQL which is present in AWS.

#Features present in Input data
Region,Channel,ItemID,Colour,Size,InvoiceDate,Total_sales

#Output data format that is moved to MySQL
Uniq_ID(Combination of Region,Channel,ItemID,Colour,Size),InvoiceDate,Forecasted_Sales
