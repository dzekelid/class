{
  "info": {
    "name": "Eventbrite Get Events  Ticket Classes Ticket Class",
    "_postman_id": "a90af80e-00b9-4d2b-beb3-dbdf2e4538c5",
    "description": "Gets and returns a single ticket_class by ID, as the key\nticket_class.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "62d11ea2-ef02-4467-ae69-b90437374975",
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
              "id": "b7d4d4b2-c7ea-4348-a0d2-a581848558ec"
            }
          ]
        },
        {
          "id": "66e950f0-62cf-4b24-be9e-3464571d1d0e",
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
              "id": "716c720e-e97b-44aa-baad-997d6aaf31e8"
            }
          ]
        },
        {
          "id": "424fbc6e-2431-424f-a57f-bc1308a28a6b",
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
              "id": "9648c05b-93a2-4625-a390-575c4652c8b0"
            }
          ]
        }
      ]
    }
  ]
}