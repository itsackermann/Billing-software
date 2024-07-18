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
>*Cid-(Customer ID)This field is used to represe

`product_details`:This table contains the basic details like price of the product,available stock of the product and total stock sold corresponding each product.

`customer_details`:This table is used to store the phone number and name of the customer along with an unique costumer id allocated to each customer based on the phone number.

`billing`:This table is used to store the product id and the quantity of product purchased temporarily.
