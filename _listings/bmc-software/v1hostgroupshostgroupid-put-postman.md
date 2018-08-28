{
  "info": {
    "name": "BMC Software API Update Hostgroup",
    "_postman_id": "0a6a22d5-d831-4d06-b893-35fc3c88aa38",
    "description": "Update a Hostgroup",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "9b9e1ea3-4678-4410-b964-e203e5d209e8",
          "name": "information-about-the-authorized-account",
          "request": {
            "url": "http://example.com/api/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the authorized account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64428281-f57b-497a-9a29-5b134e4a4137"
            }
          ]
        },
        {
          "id": "edc03081-eddc-4722-904e-0cb6cf25c477",
          "name": "get-aws-integration-status",
          "request": {
            "url": "http://example.com/api/v1/account/aws/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets AWS status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebe75739-58e2-4a63-90c3-698d27363624"
            }
          ]
        },
        {
          "id": "d7b778c9-b755-4692-82d3-eb07055e9ec6",
          "name": "delete-account-mobile-device",
          "request": {
            "url": "http://example.com/api/v1/account/mobile-devices/:accountDeviceId?accountDeviceId\nThe account device ID to delete=accountDeviceId%0AThe%20account%20device%20ID%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device from an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63af6c5b-1f74-428c-b435-ffefd6ada95d"
            }
          ]
        },
        {
          "id": "75acf9fe-d897-42c3-9a64-1b54a8042fdf",
          "name": "get-all-account-mobile-devices",
          "request": {
            "url": "http://example.com/api/v1/account/mobile-devices",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all of the devices for an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc0be5e4-4546-454e-9f7d-059223cbd35b"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "1cdcc737-f66e-4b59-9e02-79f9a8343895",
          "name": "get-all-available-action-types",
          "request": {
            "url": "http://example.com/api/v1/actions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all known action types"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e74f7735-a736-49da-bc89-afa4bf5feb48"
            }
          ]
        },
        {
          "id": "624e1bb1-634c-4383-826c-5ed42682eb5f",
          "name": "get-all-installed-actions",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all actions that are installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57acf5ec-4d34-48d1-a022-250c460536a2"
            }
          ]
        },
        {
          "id": "d775a235-55c7-406d-b5a7-712e675f315f",
          "name": "install-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an action"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0442fed-4c30-4d64-a7a9-8e103bd91195"
            }
          ]
        },
        {
          "id": "6570a646-8915-4837-b886-3655e7702d22",
          "name": "get-details-of-an-installed-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId?actionId\nName of plugin=actionId%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3eafa89-5aef-4871-b109-60037b406abd"
            }
          ]
        },
        {
          "id": "55b84e0b-6df0-4977-9733-2f14a2bb1243",
          "name": "uninstall-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Uninstalls an action and remove it from the associated alarms(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "420e6864-357e-4dcf-8628-4f9f6d16a8ae"
            }
          ]
        },
        {
          "id": "c8d940a5-54df-4064-abe0-fb898ece354f",
          "name": "get-all-alarms-using-an-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get alarms that are using this action installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e36625e5-4137-4e5b-a11d-bac03fe07996"
            }
          ]
        },
        {
          "id": "85fc14c6-b780-4e38-b36b-69047d7d5739",
          "name": "get-action",
          "request": {
            "url": "http://example.com/api/v1/actions/:action?action\nName of plugin=action%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ad2ded2-a295-4412-b2fc-e83e5f97a80e"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "e829886f-7213-4184-b555-e826c87c0542",
          "name": "get-all-alarms",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Alarms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d273dc6-6916-44c4-b976-214b0c2d2ba6"
            }
          ]
        },
        {
          "id": "91ee605f-2204-4f39-8db4-182234f1b195",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "221c2abb-bf71-4ac5-898b-079cf243d356"
            }
          ]
        },
        {
          "id": "af4141d4-6dd6-4276-812a-b18c34147aa0",
          "name": "get-alarm-by-id",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId=alarmId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2f9e3c9-049e-4fa1-9cf0-53d6a523358b"
            }
          ]
        },
        {
          "id": "7f1f8809-ae56-4e55-9ff0-14f97b48d374",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Update an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fff23f63-72d4-4ee5-9ada-9e2b759bcfce"
            }
          ]
        },
        {
          "id": "6ccff2d5-4a86-46aa-9817-4ffb6b30f7f8",
          "name": "delete-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId\nThe alarm to delete=alarmId%0AThe%20alarm%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1be10fa-af2f-47b3-880e-128b3c0fea6d"
            }
          ]
        },
        {
          "id": "7cc9d45b-daa7-4af4-acd3-b683ef05279d",
          "name": "get-alarms-by-name",
          "request": {
            "url": "http://example.com/api/v1/alarms/search?alarmName=alarmName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves alarms by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c91b972-4229-4fcc-8ada-aa64ef82e746"
            }
          ]
        },
        {
          "id": "301f8538-e072-4a88-9656-8deab443f69f",
          "name": "get-all-alarms1",
          "request": {
            "url": "http://example.com/api/v2/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Alarms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "133d5155-f0fa-4624-896b-bc64a5ff06f6"
            }
          ]
        },
        {
          "id": "297060d6-029b-4b57-a7fe-b1db28761f09",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa71cd07-2e80-4067-9fca-67391dfc04d1"
            }
          ]
        },
        {
          "id": "8700c7b7-66f5-4bd0-b746-541c362b7693",
          "name": "get-alarm-by-id1",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId=alarmId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22312601-f574-44f3-8ebd-f407253a3eb6"
            }
          ]
        },
        {
          "id": "30df1f53-ce02-438d-b7cc-a5efb3a665a7",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId integer\nThe alarm to update=alarmId%20integer%0AThe%20alarm%20to%20update",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9aa82a4-72ac-47bf-9c45-bdd35d1751ec"
            }
          ]
        },
        {
          "id": "511e75a7-bc44-4ccb-8fce-dd1d529cd167",
          "name": "delete-alarm1",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId\nThe alarm to delete=alarmId%0AThe%20alarm%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60182786-9e8f-482d-9b68-6f37d5ffce43"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "6b16ac40-0dd2-4866-ad67-428fd782aaa0",
          "name": "perform-batch",
          "request": {
            "url": "http://example.com/api/v1/batch",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows making an arbitrary set of API calls.    All calls are made in parallel.\nThe query string parameter <em>?series</em> can be used to override this behavior and call the API in series stopping at the first error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475272ce-156d-4814-a5b8-77e496ae23da"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "82b307da-2bca-4e48-ba81-43221dcd14ae",
          "name": "delete-mobile-device",
          "request": {
            "url": "http://example.com/api/v1/mobile-devices/:userDeviceId?userDeviceId\nThe user device ID to delete=userDeviceId%0AThe%20user%20device%20ID%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device from a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fcf68cc-66a2-4aac-8a80-dba5092912be"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "16673bc6-c99c-43c3-b774-22ecff0eece8",
          "name": "list-dataset",
          "request": {
            "url": "http://example.com/api/v1/datasets/*",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "*"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93f616d2-76cc-4f41-a695-9a27142564f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "b9d1ba96-7d16-42b7-85d9-bef6496ca767",
          "name": "list-events",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for events in the specified organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cf6cd43-9171-480f-8498-770b360d5737"
            }
          ]
        },
        {
          "id": "8cfbac88-f4de-428c-b14d-237118092bb3",
          "name": "create-event",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an event. Every event occurrence is persisted to the database as a RawEvent. Based on the EventFingerprint, a new Event will be created or an existing one will be de-duplicated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a011389-e692-46dc-8130-3799ff247cd3"
            }
          ]
        },
        {
          "id": "14aad6c8-8b73-4fc6-ac75-edff3b709ebb",
          "name": "list-raw-events",
          "request": {
            "url": "http://example.com/api/v1/events/raw",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Queries all event occurrences (raw events) for the specified organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d99332b-2c10-46a2-89ac-f3b5e59df678"
            }
          ]
        },
        {
          "id": "78a9350f-6166-4674-b186-524d79985451",
          "name": "get-event",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the event with the specified event id from the database."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce104ddb-203c-48b0-8073-27c97c97456f"
            }
          ]
        },
        {
          "id": "d335dc5a-213d-44b4-8054-71f366689a9e",
          "name": "get-raw-events",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id/raw",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the event occurrences (raw events) for the specified event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e39006c4-dfb5-4654-a521-a959f8b19c65"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "5830b10b-5405-4fe1-bd7e-b29d035f2345",
          "name": "get-all-hostgroups",
          "request": {
            "url": "http://example.com/api/v1/hostgroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Hostgroups in your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc7f0b1e-a7cf-40ea-a799-312dddee4eb6"
            }
          ]
        },
        {
          "id": "dfe97318-cc2c-4298-9336-78dd9480ad85",
          "name": "create-hostgroup",
          "request": {
            "url": "http://example.com/api/v1/hostgroups",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a Hostgroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1660166-64c9-4e3f-996b-a27a96e057df"
            }
          ]
        },
        {
          "id": "0e5c9402-fcef-43d0-b1db-8e383c42a778",
          "name": "search-hostgroups",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/search?name\nThe hostgroup name to search for.  Currently supported search parameters:\n\nname - search by the name of the hostgroup=name%0AThe%20hostgroup%20name%20to%20search%20for.%20%20Currently%20supported%20search%20parameters%3A%0A%0Aname%20-%20search%20by%20the%20name%20of%20the%20hostgroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches the hostgroups in your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be830a15-e020-47ae-8d53-ac4eea6592e3"
            }
          ]
        },
        {
          "id": "f9b26555-9711-4c57-89b2-9cc526f29863",
          "name": "get-hostgroup-by-id",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/:hostgroupId?hostgroupId\nThe Id of the hostgroup you are requesting=hostgroupId%0AThe%20Id%20of%20the%20hostgroup%20you%20are%20requesting",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single hostgroup by its id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65ebdec2-5765-4534-bd3b-c380db46bf33"
            }
          ]
        },
        {
          "id": "7c33fdb7-88cb-4c84-a745-bf521a5f7b7c",
          "name": "update-hostgroup",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/:hostgroupId",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a Hostgroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bae50d38-b2df-4713-83d8-fb2f7ed3cbb3"
            }
          ]
        }
      ]
    }
  ]
}