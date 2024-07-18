# Billing-software
## Overview

This project uses the following 4 tables in MySQL to implement the billing system project.

`bill_details`:This table contains the information of every bill generated as rows of the table.
>This table contains the following attributes
>
>*Invoice_number-Every bill is assigned with an unique invoice number starting from 1.
>
>*Item-This field is used to store the product ids of all purchased products in a comma separated format.For ex:"2,3,41" ->This means that the products with product id 2,3 and 41 were purchased for the current bill;
>
>*Quantity-This field contains the quantity of each purchased product in comma separated format.
>
>*Cid-(Customer ID)This field is used to represent the customer involved in the current purchase.
>
>*Price-This field is used to store the total cost of the current purchase.
>
>*Payment_Status-('U' or 'P')This field is used to indicate whether the total price of the current purchase has been paid or not.

`product_details`:This table contains the basic details like price of the product,available stock of the product and total stock sold corresponding each product.
>*pid-This field is used to store the unique product id assigned to each product. This acts helpful in separating products with same name from different brands and products with same name but different cost.
>
>*product_name-This field is used to store the name of the product.
>
>*Quantity_sold-This field is used to store the total stock of the product sold.
>
>*price_per_unit:This field is used to store the price of the unit for a basic unit of that product.For ex:For 'RICE'-50Rs/Kg.
>
>*Stock_available:This field is used to indicate the remaining available stock of the particular product.

`customer_details`:This table is used to store the phone number and name of the customer along with an unique costumer id allocated to each customer based on the phone number.
>*cid-This field is to represent each customer uniquely (assigned based on unique phone numbeers).
>
>*name-This field is used to store the name of each customer(Only the first given name for a specific phone number gets stored).
>
>*phone_

`billing`:This table is used to store the product id and the quantity of product purchased temporarily.
