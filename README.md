# crawl_newegg_site

Problem Statement:

After the decline in Bitcoin and other cryptocurrencies, the company needs to gather information about graphics cards through a website. The Data Engineer team is required to collect and analyze the information from the following category on the website: https://www.newegg.com, so that the business team can deploy a new campaign based on this data.

Description:
The data source to crawl is the following category: https://www.newegg.com/GPUs-Video-Graphics-Cards/SubCategory/ID-48?Tid=7709

1// Information to be extracted:
- ItemID
- Title
- Branding
- Rating
- Rating Count
- Price (Current Price) → Converted to a numerical format
- Shipping (Free, Not Available, or Fee Applies)
- Image URL

2// Detailed product information:
- Max Resolution
- DisplayPort
- HDMI
- DirectX
- Model
  
3// Quantity: 
All products from 100 pages (approximately 3600 products)

4// The collected information will be stored in a MySQL database:
- Add a column for total price based on the shipping fee
- Store detailed product information in JSON format
  
5// Statistical requirements (if possible, visualize the data):
- Brands providing graphics cards and the number of products from each brand.
- Price distribution of the products (What is the common price range?)
- Price distribution of products by brand
- Representation of the relationship between product price and user rating
