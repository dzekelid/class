---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/classes/{contactClassId}:
    get:
      summary: Get a contact class
      description: Gets a contact class. The ID of the contact class must be specified.
      operationId: getRestAccountsContactsClassesContactclass
      x-api-path-slug: restaccountscontactsclassescontactclassid-get
      parameters:
      - in: path
        name: contactClassId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Class
  /rest/items/sales_prices/{id}/customer_classes:
    post:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: postRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/customer_classes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
  /rest/items/sales_prices/{id}/customer_classes/{customerClassId}:
    delete:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: deleteRestItemsSalesPricesCustomerClassesCustomerclass
      x-api-path-slug: restitemssales-pricesidcustomer-classescustomerclassid-delete
      parameters:
      - in: path
        name: customerClassId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
---