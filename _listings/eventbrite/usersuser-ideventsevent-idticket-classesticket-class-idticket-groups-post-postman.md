{
  "info": {
    "name": "Eventbrite Add Users User  Events Event  Ticket Classes Ticket Class  Ticket Groups",
    "_postman_id": "42740970-1d4b-4f2b-8721-0d26539474f2",
    "description": "Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that\nbelongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.\nIf the list provided is empty, remove this ticket class from every ticket group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "e236d8c4-5c76-4335-a0aa-eed3a612d34a",
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
              "id": "6bb3b1be-3fab-44f5-ba1c-ce071cfb4e7c"
            }
          ]
        },
        {
          "id": "6b609ca9-ef87-44c4-b344-865b2828f8c1",
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
              "id": "59609bb1-5424-4078-92ac-a552342046db"
            }
          ]
        },
        {
          "id": "45566b6f-f788-4ae2-a074-5afaf6f5570f",
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
              "id": "e0a5bdd7-f05e-4040-817d-a52f7039145a"
            }
          ]
        },
        {
          "id": "29e2eb99-0134-445b-b743-dfac12dd3fa5",
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
              "id": "f6864bca-6144-46a2-a6d8-5ff28e4dd6f6"
            }
          ]
        },
        {
          "id": "8a89f94d-1e6f-4436-9422-6372d4f6e28e",
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
              "id": "e3f72eb4-baa6-4b57-9b59-89ff8528d98c"
            }
          ]
        },
        {
          "id": "34a2c424-719b-4d63-a5c6-24b65fe37fa9",
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
              "id": "2f3392eb-8efa-4ad5-a795-e66b934690b7"
            }
          ]
        },
        {
          "id": "9ae03221-0114-4d88-b367-6d357e3845b3",
          "name": "deleteEventsEventTicketClassesTicketClassTicketGroupsTicketGroup",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove the Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id from the Ticket Group identified by :ticket_group_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e8a8e51-cd1a-4dd2-aacc-f4e10f99334c"
            }
          ]
        },
        {
          "id": "f94d52c7-5042-49d3-85c3-a790cef9aadc",
          "name": "getEventsEventTicketClassesTicketClassTicketGroups",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/?status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.\nBy default, only the ticket groups that are live are shown."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66ace493-f689-4c16-999f-db982c48f8ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "5379d293-0b43-454c-8a6a-7652edb49f38",
          "name": "postUsersUserEventsEventTicketClassesTicketClassTicketGroups",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/?ticket_group_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that\nbelongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.\nIf the list provided is empty, remove this ticket class from every ticket group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff71de27-6848-4d71-aa63-d7cca7c490be"
            }
          ]
        }
      ]
    }
  ]
}