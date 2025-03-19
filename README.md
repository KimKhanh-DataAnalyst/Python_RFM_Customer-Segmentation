# Python_RFM_Customer-Segmentation
Please see the coding file attached or reach this link: https://colab.research.google.com/drive/1_WX6LpONUoPyFxfKNza9nOfvzUkt3UBi#scrollTo=ca6787be

# I. Introduction
## 1. Business question
- SuperStore is a global retail company. The Marketing Department wants to run marketing campaigns during the Christmas and New Year holidays to thank customers for their past support of the company. In addition, potential customers can be upgraded to become loyal customers.
- The Marketing Director also proposed a plan to use the RFM model in Python to segment customers and then launch appropriate marketing campaigns. Analyze the current situation of the company and give suggestions to the Marketing team
- With the retail model of Superstore company, which indicator should be most focused on in the 3 indicators R, F, and M?
## 2. Dataset
Dataset includes 4 different related tables including: transaction information, products information, returned orders of customers purchasing products from 2014 to 2017 and RFM classification

- Transaction information dataframe
  <img width="1230" alt="Image" src="https://github.com/user-attachments/assets/b58db1d4-5519-44f2-b4a9-a114a0be0e05" />[](url)

- Returned orders dataframe: We have to filter orders that were not returned before RFM anaalysis.

  <img width="498" alt="Image" src="https://github.com/user-attachments/assets/f9214240-9de9-44fd-9608-28f120b33289" />

- Segmentation dataframe: 'Product ID' is not unique because some products have same Product ID but have different Product Name => drop 'Product Name' then remove duplicate records so that 'Product ID' will be unique.

  
