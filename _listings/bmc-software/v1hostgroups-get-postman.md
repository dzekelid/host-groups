{
  "info": {
    "name": "BMC Software API Get All Hostgroups",
    "_postman_id": "4982966c-bd2c-44a0-b241-3194a271da14",
    "description": "Get all of the Hostgroups in your account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "72ece418-2333-422a-b09b-1cd56a0dc652",
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
              "id": "928730aa-68a9-4f5e-a51f-2cc86628d314"
            }
          ]
        },
        {
          "id": "9dd2e1b8-461d-4ddb-89a6-685bcbe30cf2",
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
              "id": "bbfc2e14-d56e-4909-9abb-c208c7f7f3ef"
            }
          ]
        },
        {
          "id": "c2bf70a4-dad7-4c69-8bd7-10305e5dd6f4",
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
              "id": "9fbabdb8-0168-4276-a414-fe0fe15f2e48"
            }
          ]
        },
        {
          "id": "8ffa5deb-6d3e-4f0e-af73-0b93d0f888ea",
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
              "id": "f276bae3-ad57-4e5e-b647-b453c780a71b"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "a8ab7b87-18cd-4d40-9251-f4461b5629d4",
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
              "id": "c30fdc30-9711-4610-ba68-d96a20e0246a"
            }
          ]
        },
        {
          "id": "7ca559ee-0789-475c-ad20-2fc7874347e3",
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
              "id": "60e93e45-8497-4d08-ac95-e24592628dd7"
            }
          ]
        },
        {
          "id": "2c69e009-318f-4242-9eda-449b47ad546d",
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
              "id": "6b51cee2-0b77-43fe-a3a3-de3150a944e2"
            }
          ]
        },
        {
          "id": "ef662e04-c2a8-41a5-a01e-83bb21340ebc",
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
              "id": "035e0b9f-22b2-495b-8c0c-f4ed07f3ac78"
            }
          ]
        },
        {
          "id": "271c8a7b-f9ce-413b-a731-4330ac4dca37",
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
              "id": "60e549bb-4d50-45f0-8c10-c385bf1d21ff"
            }
          ]
        },
        {
          "id": "1fad828a-741f-400e-b422-50fd832c5110",
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
              "id": "9d7bd070-4669-4909-a11d-7beacd18119e"
            }
          ]
        },
        {
          "id": "cc1d103c-b29e-41eb-a6e5-2586d84fd9b7",
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
              "id": "d561241f-3e37-4d3a-8450-e7912add07aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "7a5eaab7-2c13-470b-ac79-d99f04f8d4b2",
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
              "id": "aba2e275-c03f-4d18-8614-c242d20142be"
            }
          ]
        },
        {
          "id": "0b1fa327-5907-408d-9400-fc884dec225a",
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
              "id": "3fb599f1-46da-47d4-8199-54b44445b047"
            }
          ]
        },
        {
          "id": "70490c78-d59f-4d57-b648-268ff636bf9d",
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
              "id": "153fe63d-0d6d-4777-82cb-ef8aa42b0e8d"
            }
          ]
        },
        {
          "id": "d5729716-eb2e-4c85-84eb-ad699492ee16",
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
              "id": "04e7cb1a-561f-46b6-b157-b32f5ca9a237"
            }
          ]
        },
        {
          "id": "3a5c798f-82be-45d5-8f27-21aeee928f13",
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
              "id": "2777bc87-ed0a-4b72-9d93-cb1a59fa350d"
            }
          ]
        },
        {
          "id": "730427c1-5dcb-4728-982b-18520fdf23f1",
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
              "id": "2a5fb42a-813d-418c-9d31-2b680d8e3ed7"
            }
          ]
        },
        {
          "id": "aeef5700-506e-41ed-97ea-c14164e27541",
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
              "id": "d7c8fad3-e70c-41dd-9047-aa8750a94db5"
            }
          ]
        },
        {
          "id": "00281ced-342e-42cf-a8fb-9add49d4e30f",
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
              "id": "b41cebe2-768e-4036-855b-d729bdca5717"
            }
          ]
        },
        {
          "id": "b48084a8-10f0-487c-82a8-7a1e45bcc324",
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
              "id": "23030be4-5646-4a6b-b292-206f2086f038"
            }
          ]
        },
        {
          "id": "d196bb4b-f7c3-41ff-984d-dc971ae5550e",
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
              "id": "2904b4fc-3899-46c8-afca-d945bdb68903"
            }
          ]
        },
        {
          "id": "c54b3e04-ed3e-4bb7-b887-2aabfdf46675",
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
              "id": "1185cdd4-662d-48b4-97eb-7d51dd30e5a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "342a00a5-e67d-4219-b600-8862f2c385b3",
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
              "id": "3a24e4c1-2409-44e4-b6fe-5d1a118561ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "3cd68d32-f8fc-4293-b2d5-36b71ddb9274",
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
              "id": "bf492460-7d57-42ad-95a0-350643c2949f"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "4b46b63d-7eaa-41de-8195-56a69e536530",
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
              "id": "10c5efd1-859d-453a-add5-c3a01ad36147"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "4d5d7db6-3203-4de0-a7ee-51e5c88d179e",
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
              "id": "6646b9dc-6fe4-4d75-ab39-e7240b195d59"
            }
          ]
        },
        {
          "id": "ed4ab0af-9b4d-4f87-b79d-95a49f4814fd",
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
              "id": "d0aa76ab-ed5c-4609-b841-01b7f4d5ff16"
            }
          ]
        },
        {
          "id": "99bf67bd-df7b-4f14-bb8e-a2606532c94a",
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
              "id": "f9a0535c-a81a-4210-8281-f605ea697b28"
            }
          ]
        },
        {
          "id": "e4d1d2f5-6da6-4607-b7ab-01deb8cf87b7",
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
              "id": "0a83cf3f-4121-4d29-ad74-595ea8545c37"
            }
          ]
        },
        {
          "id": "d4313721-1319-44d9-b585-bf0356a3eccc",
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
              "id": "0847e638-32aa-4b3b-879a-9964da905808"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "1a85daca-cbf0-4b9e-b177-eef1bec4c7dc",
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
              "id": "89f732e9-7b93-4222-9ab2-3e08da7e4bd0"
            }
          ]
        }
      ]
    }
  ]
}