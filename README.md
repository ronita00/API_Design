# API design description
---
  - [For creating products API](#for-creating-products-api)
    - [Creat product: POST "/api/v1/products"](#creat-product-post-apiv1products)
    - [Get all product: GET"/api/v1/products"](#get-all-product-getapiv1products)
    - [Update a product:PUT"/api/v1/products/{id}"](#update-a-productputapiv1productsid)
    - [DELETE products:DELETE"/api/v1/produc{id}"](#delete-productsdeleteapiv1producid)

## For creating products API
### Creat product: POST "/api/v1/products"


                Authn: Basic/Baerer Token
                Body: JSON Data
                Respons: 
                    1.Body: Optional
                    2.Code:
                            200 Ok
                            400 Bad request
                            401 Unauthorized
                            500 Serverside error


### Get all product: GET"/api/v1/products"
                Authn: Basic/Baerer Token
                Body: None
                Respons: 
                    1.Body: List of product JSON
                    2.Code:
                            200 Ok
                            401 Unauthorized
                            500 Serverside error

### Update a product:PUT"/api/v1/products/{id}"
                Authn:Basic/Baerer Token
                Body:PUT->Full obj,PAECH->Partial obj
                Respons: 
                1.Body:Uodated product JSON
                2.Code:
                        200 Ok
                        400 Bad Request
                        401 Unauthorized
                        404 Not found
                        500 Serverside error


### DELETE products:DELETE"/api/v1/produc{id}"

                Author:Basic/Bearer token
                Body:None
                Response:
                    1.Body:=>Delete json obj/empty
                    2.code:
                        200 ok
                        401 unathenticated
                        404 Not Found
                        500 server error
                        
