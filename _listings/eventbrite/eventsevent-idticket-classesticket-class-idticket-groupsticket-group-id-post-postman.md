{
  "info": {
    "name": "Eventbrite Add Events Event  Ticket Classes Ticket Class  Ticket Groups Ticket Group",
    "_postman_id": "2b2a1835-d456-44fc-b310-7e44681155ca",
    "description": "Add the Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id to the Ticket Group identified by :ticket_group_id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "30b62925-3ab5-4229-9c48-a1538174d2f7",
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
              "id": "2b68bb4c-92b1-4ab9-87a3-e6ee1dbfe7b0"
            }
          ]
        },
        {
          "id": "7952281c-f691-4cd1-ab7a-bcfe6233fb36",
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
              "id": "ad7f561e-b629-4d7a-bc64-ac6d94446ecb"
            }
          ]
        },
        {
          "id": "1576a1cb-b81f-459d-bee9-93e93375dbf3",
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
              "id": "2deb7e39-4f1b-40d6-ab23-40e29f01ddb0"
            }
          ]
        },
        {
          "id": "2b9216b9-8bf1-4754-bb6f-ce4f742c070b",
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
              "id": "d53e1fd3-4bb8-484e-9fc3-468906009cdf"
            }
          ]
        },
        {
          "id": "28fda14a-97c3-4430-b679-d4fddeb1afbf",
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
              "id": "e15f5768-62e4-46a4-afc7-d95fa9fa13d1"
            }
          ]
        },
        {
          "id": "c61a7204-dc13-4796-8a09-a520d9d171de",
          "name": "postEventsEventTicketClassesTicketClassTicketGroupsTicketGroup",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id to the Ticket Group identified by :ticket_group_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4caf30d-5b9c-4355-868e-d72130e212f2"
            }
          ]
        }
      ]
    }
  ]
}