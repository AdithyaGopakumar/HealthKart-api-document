## page 1 home page

- all products
  https://healthkart-render-api.onrender.com/allproducts
- brands api
  https://healthkart-render-api.onrender.com/brands
- category api
  https://healthkart-render-api.onrender.com/categories
- flash sale api
  https://healthkart-render-api.onrender.com/allproducts/flashsale
- trending now api
  https://healthkart-render-api.onrender.com/allproducts/trending
- tending in whey protien api
  https://healthkart-render-api.onrender.com/allproducts/trendingwhey
- gaining supplements api
  https://healthkart-render-api.onrender.com/allproducts/gainers

## page 2 individual brand page

- products per brand api
  https://healthkart-render-api.onrender.com/allproducts?brandId=1
- products based on category
  https://healthkart-render-api.onrender.com/allproducts?categoryId=5
- products based on brand and category
  https://healthkart-render-api.onrender.com/filter/1?categoryId=1
- products based on category and brand
  not required
- products based on brand category and price
  https://healthkart-render-api.onrender.com/filter/1?categoryId=1&hcost=3000&lcost=2000
- product on the basis of cost(hcost and lcost)
  https://healthkart-render-api.onrender.com/filter/1?hcost=2000&lcost=1000
- sort on the basis of cost(high and low)
  by default it is in accending order
- for descending order
  https://healthkart-render-api.onrender.com/filter/7?categoryId=2&sort=-1

## page 3 individual product page

- details of the product api
  https://healthkart-render-api.onrender.com/brands/50
- Add to cart(POST)
  (same as page 4 cart)

## page 4 cart

- cart details(POST)
  https://healthkart-render-api.onrender.com/cart
  body ={

      "id": [
          11,22,33,44,55
      ]

}

- place order(POST)
  https://healthkart-render-api.onrender.com/placeOrder
  body ={

          "_id": "636f392457424adaec829aaa",
          "order_id": 1,
          "name": "Adithya Gopakumar",
          "email": "adi@123.com",
          "address": "home, city, pin",
          "phone": 837564056,
          "total": 2354,
          "items": [
              1,
              32,
              51
          ]
      }

## page 5 order confimation page

- list of orders
  https://healthkart-render-api.onrender.com/orders
- list of orders with respect to email
  https://healthkart-render-api.onrender.com/orders?email=adi@123.com
- update payment details(PUT)
  https://healthkart-render-api.onrender.com/updateOrder/1
  body = {

        "status": "Txn Success",
        "bank_name": "HDFC",
        "date": "16/11/2022"

}

- delete order(DELETE)(just pass the order's \_id)
  https://healthkart-render-api.onrender.com/deleteOrder/637b83e3296f176e5d941ac9
