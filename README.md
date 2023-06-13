# KmeansClusteringCustomerSegmentation-Unsupervised-Learning-
## Background
A small e-commerce company want to understand its customers better using Machine Learning to target their loyalty program and promotion campaigns etc. Analyze the dataset provided (which is purposely kept small for exploration purpose).
## Dataset Introduction
The dataset consists of 200 cases, in .csv format and with the following data dictionary:  
**CustomerID:** a unique ID of each customer in sequence   
**Gender:** male or female.   
**Age:** reported age of customer.   
**Income:** annual income (x HK$1,000).  
**SpendingScore:** score summarizing the spending of the customer (1-100), higher means “better”. 
## Process
In this customer dataset, I conducted exploratory data analysis (EDA) to gain insights into the customers' characteristics and lay the groundwork for model building. Through EDA, I analyzed single attribute distributions, two-dimensional attribute relationships, and three-dimensional attribute relationships.
The analysis revealed several important findings. Age showed clear relationships with SpendingScore, while SpendingScore demonstrated a strong relationship with Income. The dataset indicated that the company has a relatively stable customer base with a steady development trend. To drive future growth, it is essential to formulate different marketing and operational strategies for different customer segments.
## K-means algorithm
To address the business problem of understanding the company's customers and defining a customer segmentation strategy, I employed the K-means clustering algorithm. I built 3 models based on different attribute combinations: Age-SpendingScore, Income-SpendingScore, and Age-Income-SpendingScore.
### First Model
1. The first model, based on Age and SpendingScore, divided customers into four groups and focused on age and purchasing power. This segmentation is suitable when the company wants to launch and market new products.
<img width="504" alt="image" src="https://github.com/TracyCJY/Customer-Analysis-Unsupervised-Learning-/assets/126844450/e6163d5b-7a1a-4435-a72f-0fc851d2190d">    

### Business Insights on the First Model    
Based on the Age and SpendingScore two attributes, customers can be divided into four segments:   
● Group 0 is Young People but with High Spending Score    
● Group 1 is Middle Aged People with Low Spending Score   
● Group 2 is Old People with medium Spending Score    
● Group 3 is Young People with Low Spending Score   
● For Group 0 Young people with High Spending Score, they are compulsory customers, companies should use some new and trendy products to attract them.    
For Group 3 Young People with Low Spending Score, company should use more discount methods to stimulate purchasing orders.   
For Group 1&2, they are middle contribution customers, it is important to maintain them.    
### Second Model    
2. The second model, based on Income and SpendingScore, classified customers into five groups, emphasizing income level and purchasing power. This segmentation is beneficial for improving the company's Gross Merchandise Value (GMV) or Orders performance.      
<img width="542" alt="image" src="https://github.com/TracyCJY/Customer-Analysis-Unsupervised-Learning-/assets/126844450/5b26f16d-d489-4dd7-9cca-0fd791a9a17f">      

### Business Insights on the Second Model     
Based on the Income and SpendingScore two attributes, customers can be divided into five segments:     
● Group 0 is Low Income but with High Spending Score      
● Group 1 is Middle Income with Middle Spending Score     
● Group 2 is High Income with Low Spending Score      
● Group 3 is High Income with High Spending Score   
● Group 4 is Low Income and with Low Spending Score   
All High Spending Score customers, companies should launch some marketing method with more high price products to attract people to buy and therefore to increase the company's GMV.     
In terms of Income features of customers, the most important considerations is the company’s ATV(Average Transaction Value)   
### Third Model
3. The third model, based on Age, Income, and SpendingScore, segmented customers into six groups, providing a comprehensive customer profile. This segmentation helps build detailed customer profiles for better user management.    
<img width="362" alt="image" src="https://github.com/TracyCJY/Customer-Analysis-Unsupervised-Learning-/assets/126844450/41ea652e-94a7-4893-9c69-9687bb2da1a9">      

### Business Insights on the Third Model    
● Group 0 is Impulse Consumers: Average age is 27 years old, Income 173, SpendingScore is 78. This is mainly young people with average income but high consumption score    
● Group 1 is Important to Keep Consumers: Average age is 55 years old, Income 354, SpendingScore is 50. This is mainly middle-aged and elderly people with middle income and consumption scores   
● Group 2 is Important Value Consumers: Average age is 33 years old, Income 562, SpendingScore is 82. This is mainly middle-aged people, with high income and consumption scores, belonging to the optimal customer group.    
● Group 3 is Prudent Consumers: Average age is 45 years old, Income 585, SpendingScore is 19. This is mainly middle-aged people with high income but low consumption score.   
● Group 4 is Important Development Consumers: Average age is 25 years old, Income 376, SpendingScore is 44. This is mainly young people, with middle income and consumption scores, they have great potential.    
● Group 5 is Average Value Consumers : Average age is 45 years old, Income 171, SpendingScore is 20. This is mainly middle-aged people, but with low income and consumption scores. They are the least valuable customers   
Maintenance customer is the biggest customer segmentation, which means the company has the most important to keep the customers.    
Average customer is the least customer segmentation, which means the company has the least average value consumers    
## Conclusion
Throughout the analysis, I provided business insights and recommendations for each model. These insights ranged from targeting specific customer groups with new and trendy products to stimulating purchasing orders through discount methods. The analysis also highlighted the importance of Average Transaction Value (ATV) and maintaining high-spending customers. In conclusion, customer segmentation is crucial for e-commerce companies to enhance their performance and future strategic management. By using different clustering models, businesses can tailor their marketing and operational strategies to specific customer segments, leading to improved customer engagement and increased performance.      
