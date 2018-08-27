{
  "info": {
    "name": "Eventbrite Delete Events  Ticket Classes Ticket Class",
    "_postman_id": "14f40d1b-854f-42fe-95d6-e448f9bc8fcc",
    "description": "Deletes the ticket class. Returns {&quot;deleted&quot;: true}.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "fe3c102c-07a5-4c44-8ad2-cdb5648b8435",
          "name": "getEventsTicketClasses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/ticket_classes/"
              ],
              "query": [
                {
                  "key": "pos",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response with a key of\nticket_classes, containing a list of ticket_class."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e01747e-0aa9-4c57-8f93-e0b339260287"
            }
          ]
        },
        {
          "id": "70469d78-d9b0-4010-8b82-4b40ae21d1f5",
          "name": "postEventsTicketClasses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/ticket_classes/"
              ],
              "query": [
                {
                  "key": "ticket_class.auto_hide",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.auto_hide_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.auto_hide_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.cost",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.donation",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.free",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.hide_description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.include_fee",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.maximum_quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.minimum_quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.order_confirmation_message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.quantity_total",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_channels",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_start_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.split_fee",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ticket class, returning the result as a ticket_class\nunder the key ticket_class."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4deae579-2be8-4dee-8dbd-d3edb57eeff3"
            }
          ]
        },
        {
          "id": "74e15b57-11be-4f26-9169-591ec3129304",
          "name": "getEventsTicketClassesTicketClass",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/ticket_classes/:ticket_class_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets and returns a single ticket_class by ID, as the key\nticket_class."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c72e5c1-a1a1-4610-b8ce-6cb66ebf205d"
            }
          ]
        },
        {
          "id": "ac4edc1f-47a1-4ebe-a560-e7c90edf3bd1",
          "name": "postEventsTicketClassesTicketClass",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/ticket_classes/:ticket_class_id/"
              ],
              "query": [
                {
                  "key": "ticket_class.auto_hide",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.auto_hide_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.auto_hide_before",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.cost",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.donation",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.free",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.hide_description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.include_fee",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.maximum_quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.minimum_quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.order_confirmation_message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.quantity_total",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_channels",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.sales_start_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ticket_class.split_fee",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an existing ticket class, returning the updated result as a ticket_class under the key ticket_class."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1ac04c6-6c13-4580-974f-6967f6599a39"
            }
          ]
        },
        {
          "id": "8a013b44-c756-48e0-b010-325e6fef5d9e",
          "name": "deleteEventsTicketClassesTicketClass",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "events/:id/ticket_classes/:ticket_class_id/"
              ],
              "query": [
                {
                  "key": "break_dependency",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the ticket class. Returns {&quot;deleted&quot;: true}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72522fd3-c7e2-4b5a-a525-a6c7bfeebd19"
            }
          ]
        }
      ]
    }
  ]
}