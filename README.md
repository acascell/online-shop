# online-shop
On-line web-shop using Django Celery RabbitMQ

### 🚀 Overview
The online shop enables client to browse products, add them to the cart, apply discounts,
go through the checkout process, pay with credit crt and obtain an invoice.

![cart1.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fcart1.png)
![cart2.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fcart2.png)
![checkot.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fcheckot.png)
![main2.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fmain2.png)
![main_1.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fmain_1.png)
![payment_confirmations_logs.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fpayment_confirmations_logs.png)
![stripe.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fstripe.png)
![successful.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fsuccessful.png)

### 🍁 Model definition
![model.png](myshop%2Fshop%2Fstatic%2Fscreenshots%2Fmodel.png)

### ✨ Features
- Front-end defined using simple html/css with fine-grained design including navbar/sub-bar, header, sidebar, 
product detail, order info, form payment
- Built product catalog (Drinks shop: tea,coffee,ginseng) based on predefined models product and category.
- Catalogue view defined using function based views and django template rendering offering a clear and concise 
catalogue space
- Built shopping cart allowing user to store and buy products including actions/methods such: "add" "remove"
"save" "get total price" "clear". 
- Utilised django session framework as middleware to store cart data

## Urls router endpoint

    - "admin/"
    - "cart/"
        "add/<int:product_id>/"
        "remove/<int:product_id>/"
    - "orders/"
        "create/"
        "admin/order/<int:order_id>/"
    - "payment/"
        "process/"
        "completed/"
        "canceled/"
        "webhook/"
    - "coupons/"
        "apply/"


### 🚀 Technology Stack
- python 3.9
- django 4.0
- sqlite
- html/css/javascript/AJAX
- docker
- redis
- rabbitMQ
- celery/flower
- pyllow
- weasyprint


### 🔎 TODO
- Add internationalization LN_EN
- export pdf
- replace django session with memcache to store user session data