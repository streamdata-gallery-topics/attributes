---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Catalog Product Attributes
  description: Get catalog product attributes.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/{cartId}/attributes:
    put:
      summary: Put Cart Attributes
      description: Put cart attributes.
      operationId: putCartCartAttributes
      x-api-path-slug: cartcartidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
    delete:
      summary: Delete Cart Attributes
      description: Delete cart attributes.
      operationId: deleteCartCartAttributes
      x-api-path-slug: cartcartidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
  /cart/{cartId}/item/{itemId}/attributes:
    put:
      summary: Put Cart Item Attributes
      description: Put cart item attributes.
      operationId: putCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
    delete:
      summary: Delete Cart Item Attributes
      description: Delete cart item attributes.
      operationId: deleteCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
  /catalog/category/{categoryId}/attributes:
    get:
      summary: Get Catalog Category Attributes
      description: Get catalog category attributes.
      operationId: getCatalogCategoryCategoryAttributes
      x-api-path-slug: catalogcategorycategoryidattributes-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Attributes
  /catalog/product/{productId}/attributes:
    get:
      summary: Get Catalog Product Attributes
      description: Get catalog product attributes.
      operationId: getCatalogProductProductAttributes
      x-api-path-slug: catalogproductproductidattributes-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Attributes
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---