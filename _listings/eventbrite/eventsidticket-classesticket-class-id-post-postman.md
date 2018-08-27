{
  "info": {
    "name": "Eventbrite Add Events  Ticket Classes Ticket Class",
    "_postman_id": "f5433598-a899-4ae7-ae66-e274e0bf2d5e",
    "description": "Updates an existing ticket class, returning the updated result as a ticket_class under the key ticket_class.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "d2753980-ca0b-46cc-81d5-f5a70572f380",
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
              "id": "00702598-c503-46d5-ae9b-7a8997fc3a33"
            }
          ]
        },
        {
          "id": "cd9735a1-c1b9-4473-b7ca-083482f74f9c",
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
              "id": "8cb96808-4af6-4d85-a6a2-8da174f30ca1"
            }
          ]
        },
        {
          "id": "713b99c5-efca-4333-a074-c8b019962958",
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
              "id": "d6a56815-bf15-4f49-9d20-e926a04fb132"
            }
          ]
        },
        {
          "id": "6889d2dc-50a0-4887-9430-6c526db3f696",
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
              "id": "6431478d-45c5-4c68-b2b5-6379ac47285b"
            }
          ]
        }
      ]
    }
  ]
}