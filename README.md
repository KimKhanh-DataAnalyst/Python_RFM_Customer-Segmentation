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

  <img width="670" alt="Image" src="https://github.com/user-attachments/assets/419d0b45-ac5e-4d55-a0c7-502fbf7e8065" />

- Products dataframe: We have to split each RFM score into single rows

<img width="517" alt="Image" src="https://github.com/user-attachments/assets/b86a3c08-9f0b-4714-a59e-1a1c53710edd" />

<img width="515" alt="Image" src="https://github.com/user-attachments/assets/bf2530b6-4895-4b26-b966-8f2ccfc0ea2a" />

<img width="384" alt="Image" src="https://github.com/user-attachments/assets/13d2842f-5e89-494b-995f-8c221f25dd38" />

<img width="381" alt="Image" src="https://github.com/user-attachments/assets/64f28ec1-2977-4d7c-913e-282f3ace972d" />

<img width="645" alt="Image" src="https://github.com/user-attachments/assets/693f1b54-b631-45c1-8fd5-f903159d798f" />

<img width="656" alt="Image" src="https://github.com/user-attachments/assets/cc49ef59-a09b-4825-a2b2-c36575bd01af" />
