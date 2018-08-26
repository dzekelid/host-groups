{
  "info": {
    "name": "BMC Software API Create Hostgroup",
    "_postman_id": "9449ea54-a507-4022-9385-909f86599906",
    "description": "Create a Hostgroup",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "667d9717-c6c5-4bf1-8e5e-d5dc937c6d01",
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
              "id": "d9e873db-8832-46d0-9241-1c5925425326"
            }
          ]
        },
        {
          "id": "bbbef79c-6b8f-4eb7-b63d-ff041673aa50",
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
              "id": "8d1683eb-25ac-4ff7-b5eb-8f723b8128dc"
            }
          ]
        },
        {
          "id": "9570ac7f-eacd-4546-8df8-e47dfa4ac20d",
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
              "id": "9e623b8a-5a99-453f-bb86-9e917cbca99f"
            }
          ]
        },
        {
          "id": "4ecb9e48-1a06-4746-90b8-040028393448",
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
              "id": "fc69ee72-f644-409e-8b8e-7fd152cc2c49"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "3dc64231-fe8e-4370-bd58-418cd1752084",
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
              "id": "21162a55-8082-44b1-ac86-4e8dfecec5bb"
            }
          ]
        },
        {
          "id": "665b7cce-942c-4617-b612-4ee58dd94d7d",
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
              "id": "95b62ec4-cba9-4e08-ab43-0bafac9546c5"
            }
          ]
        },
        {
          "id": "0114f829-3519-40e2-aa1c-301c5fdebc4b",
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
              "id": "658672b2-0bb0-4028-9865-4f75e4553213"
            }
          ]
        },
        {
          "id": "9652c5d3-a688-4e21-904a-c3c09337b877",
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
              "id": "42d58d8e-5e5c-47d5-b183-423219ab9d96"
            }
          ]
        },
        {
          "id": "a4b45e8c-36d0-4578-9d6c-21ffa7fa3864",
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
              "id": "54d40cc1-97b9-4796-b0d0-651fecc3bc3a"
            }
          ]
        },
        {
          "id": "9b0687d3-2125-4965-82e0-6961121be7a0",
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
              "id": "8a7b8dd3-2555-49e5-a1c7-c5983219c82c"
            }
          ]
        },
        {
          "id": "3e1161b2-f752-4e6c-a5fe-c9c2be3c1989",
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
              "id": "b84a1253-953c-430a-97d6-7b8bf45b325e"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "a4933a04-d907-427f-bfc7-4e712ddb1804",
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
              "id": "5b0e230a-0a2b-4beb-9930-45a6d8846463"
            }
          ]
        },
        {
          "id": "3af28868-df51-4d64-961e-445a4ed0f58f",
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
              "id": "476e41f1-5212-4952-8299-65b7a5bfd6f9"
            }
          ]
        },
        {
          "id": "0227641b-f3b6-4bfe-b38a-343aaf8f4458",
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
              "id": "7e2bdf2a-a799-4fdf-98ec-06d2ca8518ed"
            }
          ]
        },
        {
          "id": "ce93d602-cbb6-443f-9f19-30da1ff2013b",
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
              "id": "67da93c9-c26c-4514-b797-c1cf2168759d"
            }
          ]
        },
        {
          "id": "d813f7f3-45d2-40c8-9f12-15c480e5cc9d",
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
              "id": "0195a970-6c67-4888-a78d-006dfd05344e"
            }
          ]
        },
        {
          "id": "48306a72-8070-4c38-9343-ed9191b3cca1",
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
              "id": "4a253cad-7e14-4fad-b0e4-ae3fabbc717e"
            }
          ]
        },
        {
          "id": "2f1849eb-5cdd-4695-9695-f843fc457d86",
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
              "id": "eb6b14c2-5efa-40c5-b4bf-5822da229708"
            }
          ]
        },
        {
          "id": "f7ee5056-8625-49e5-8ca4-b0831849570c",
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
              "id": "91f353f1-d13e-45be-b041-8cac0df6c61c"
            }
          ]
        },
        {
          "id": "e95f2a1b-01db-4532-a580-c1d3b5b78387",
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
              "id": "470ed7c7-3097-4df5-aaf7-e1a41d2d6484"
            }
          ]
        },
        {
          "id": "1a5e5125-237e-4147-94ef-b4efd68230d1",
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
              "id": "d5d54ff4-e91c-4a16-bc6e-9de0ac28afd0"
            }
          ]
        },
        {
          "id": "84e7c6d0-b91a-4972-aa6c-fee439bf7e36",
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
              "id": "1200a949-0c3a-4e0a-9c09-56b33dda68fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "130f36ca-584d-409a-92e9-5e70cfc4672a",
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
              "id": "5c19d6e8-2d4f-4600-8ee4-0c4abe3d5dd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "8b418fb5-db4a-4ed5-bf4e-32955aaa03ee",
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
              "id": "361f4b81-d5b3-4e69-bac9-1de12e978781"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "7cbbbf6b-afaa-4761-84fe-6fe7d5517c71",
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
              "id": "2a458cf6-c70f-449e-a90d-9e4311906994"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "04a63186-169d-4c4e-84f1-a8fb6d967c26",
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
              "id": "10017d42-dd1a-48db-acbb-6ebe760f0923"
            }
          ]
        },
        {
          "id": "5941db70-2604-44c7-9da9-da7be4f96b5e",
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
              "id": "07be7ab9-0f23-4664-839e-5f779870af17"
            }
          ]
        },
        {
          "id": "67f3ca14-0824-4777-8971-4f157fa146b0",
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
              "id": "e569aae6-4346-4ae0-920c-ed9f77ae6dea"
            }
          ]
        },
        {
          "id": "d06fafc6-aa38-43d1-a01a-06cf5ac08c1a",
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
              "id": "c9bf2648-ee7e-4f9d-94b8-d2684b6a9d2d"
            }
          ]
        },
        {
          "id": "b8e9aaa4-d97d-494e-ab99-4e3f2a5cd530",
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
              "id": "218caef6-db18-47df-a92b-b89b5f2b6b1f"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "cde7aa18-778f-49d7-b034-efda5910e669",
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
              "id": "f28b9f62-d141-4b9a-849a-b57c6705bcce"
            }
          ]
        },
        {
          "id": "953b4a51-57d4-4ebe-8c6c-5c39bb77d0ad",
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
              "id": "0891e359-6256-40df-a8f9-c25c597b1d54"
            }
          ]
        },
        {
          "id": "6a8e5332-f298-4492-8c27-3ef528377ad7",
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
              "id": "ba2d09a2-40d9-4169-b2c5-4cceae6f2221"
            }
          ]
        },
        {
          "id": "3e4bb0ef-4221-41ba-a07b-459cfa30f31c",
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
              "id": "a36db6ab-9da9-48fe-bba5-149bf8df8cd2"
            }
          ]
        }
      ]
    }
  ]
}