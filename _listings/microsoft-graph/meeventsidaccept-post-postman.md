{
  "info": {
    "name": "Microsoft Graph API Event Accept",
    "_postman_id": "e360a43b-9fea-4d7a-bc10-c0eb7e32e9dd",
    "description": "event: accept Accept the specified event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachment",
      "item": [
        {
          "id": "acecb3f3-ff3a-4a03-99ab-36cb1afbb3ce",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd2d92e8-2d82-47e7-8f95-cfc3214c0274"
            }
          ]
        },
        {
          "id": "afd112d9-6f42-4e51-84b9-029fa18346da",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d8fa6fa-8fc5-4ea9-b8da-7e8e3c52e9c7"
            }
          ]
        },
        {
          "id": "93c5b879-d28e-4f59-8e5f-87bbaee39d27",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eec40683-f6f2-42d7-9376-0bf46002eac2"
            }
          ]
        },
        {
          "id": "9775d9be-5724-4466-9095-f918d40083c1",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendar/:id/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f879f890-ad77-4296-a102-25f90be25d0c"
            }
          ]
        },
        {
          "id": "a3deb367-05e1-47b1-8fca-0ce23130a3d5",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa2ae9c4-8f28-4fa8-8213-583d631f49d0"
            }
          ]
        },
        {
          "id": "578a9444-81cc-4226-a1f3-2a5dddb6ff89",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e384114c-9cbb-414e-af91-bad6e7adbfac"
            }
          ]
        },
        {
          "id": "4b180deb-dff6-480c-b714-9e0e6cd5bb3f",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25ee1c9a-ac77-40cb-b82f-5b9f5ecabdb1"
            }
          ]
        },
        {
          "id": "94469220-4baa-40b6-ad0d-52742a98fe52",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5638c923-0e3c-4eb7-97c6-28399f0dcb6e"
            }
          ]
        },
        {
          "id": "167b61f2-67ac-478a-87d0-76f6db7d0cdb",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroup/calendars/:id/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47906e6b-a072-4a4f-8d16-f4871e935133"
            }
          ]
        },
        {
          "id": "8251d577-fe72-4613-b316-037c6ea2a008",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroup/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a74cb43e-14f8-4981-b933-57d422546418"
            }
          ]
        },
        {
          "id": "1468afc8-3e51-4fa4-9d72-05e92f414023",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22c2d2f2-85ce-4109-ba25-22f9465ba523"
            }
          ]
        },
        {
          "id": "9f9afb54-aa73-4dc5-a83e-d0a3ee0e9ee4",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c5ff837-98b8-431a-94e3-87ae1e2f0ce3"
            }
          ]
        },
        {
          "id": "2c1d9477-c3c6-40ae-8c2c-67f94c1b54f2",
          "name": "GetAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/messages/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5b3740b-68bc-44fd-97a6-bf8b23582d64"
            }
          ]
        },
        {
          "id": "d75ce52a-c2a9-40ae-a431-b0272b0a4a43",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd94560-9668-4de0-bd47-6ff51286c807"
            }
          ]
        },
        {
          "id": "63f51c01-1fa1-405e-abb8-257f9c6842e8",
          "name": "GetAttachment8",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/messages/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af16c08d-d28d-4cc9-8157-5e70da3e5224"
            }
          ]
        },
        {
          "id": "bbd3e529-0332-40cc-bb95-f6c8812bc3d4",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe21f9b9-15e3-4168-b622-fe67589dda0f"
            }
          ]
        },
        {
          "id": "04158acd-fdd4-4354-947a-14c8d4bb46de",
          "name": "GetAttachment9",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/threads/:id/posts/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "366b6e4c-d0a8-40aa-9964-e34c033b82ef"
            }
          ]
        },
        {
          "id": "5143789c-0f32-485d-8226-31dcee5ae6ba",
          "name": "GetAttachment10",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/conversations/:id/threads/:id/posts/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10c0bc0b-f7b7-420a-a443-b2e41d736a02"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "221c341f-d3e2-4389-899d-f676deeae213",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/childFolders/:id/.../messages/:id/attachments/:id"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "957f2848-2e26-46c3-a982-e7d291c278e4"
            }
          ]
        },
        {
          "id": "7fa671f8-3e37-4a64-9018-c115aa60cb70",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/childFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a7bcb69-72ec-461b-ac26-cf1d05dfb4a1"
            }
          ]
        },
        {
          "id": "1fb0ad01-1d0a-4d71-a55c-bcdce8b6ff85",
          "name": "ListCalendarView",
          "request": {
            "url": "http://graph.microsoft.com/me/calendar/calendarView?endDateTime=endDateTime&startDateTime=startDateTime",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "443c5526-f6d3-42c1-a6a2-10cfc0148d35"
            }
          ]
        },
        {
          "id": "a87bb011-f74b-4d4a-99ee-fb5863a8ce0c",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99df1435-cab3-45f4-b6ac-1f6512dfabab"
            }
          ]
        },
        {
          "id": "4203d3b6-6016-4da8-8fb5-38b9722b89cc",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
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
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b098bc08-f78b-4f2a-92bf-456a59d72344"
            }
          ]
        },
        {
          "id": "1778560b-0a5e-46c0-a3d6-9f617866b13e",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a988485b-3176-4551-9109-2ab8b6f5ed83"
            }
          ]
        },
        {
          "id": "669b189e-328e-4d8b-8baf-ee8ef427bc25",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90a219f8-d6fc-482c-8152-da6faa334264"
            }
          ]
        },
        {
          "id": "b0c9cd1b-e90c-4c51-afe5-75b3f75228d1",
          "name": "ListCalendarView1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroup/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d60173f-b353-4cbb-8407-5eb58be40187"
            }
          ]
        },
        {
          "id": "867d31d5-84d5-4646-a3bf-29fd026ee114",
          "name": "ListCalendarView1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroup/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b298488-5e6e-4ce0-9af2-bec02d623e50"
            }
          ]
        },
        {
          "id": "7b6b2f46-4587-4c07-8539-6c8a82da0937",
          "name": "ListCalendarView2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroups/:id/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86773ac6-5b38-4110-8376-c064154a59f4"
            }
          ]
        },
        {
          "id": "fa3e0b88-4169-4e9c-b96b-4a371e61f601",
          "name": "ListCalendarView2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroups/:id/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45b09ba2-f4f9-4583-ac24-7a94a6187663"
            }
          ]
        },
        {
          "id": "ed029012-a05a-4e16-a77d-a5773a121dda",
          "name": "ListEvents",
          "request": {
            "url": "http://graph.microsoft.com/me/calendar/events",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2957214-8e0c-4391-81d1-79d87f324e99"
            }
          ]
        },
        {
          "id": "f698c627-61ae-49a5-987c-9503c1b98a50",
          "name": "ListEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7f85999-3024-454b-9f6c-1635734f63d0"
            }
          ]
        },
        {
          "id": "86e36dcf-77da-4b21-9f3b-93896b616a2a",
          "name": "ListEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events"
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
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of event objects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a3b156e-1e7c-4ad7-945c-bb8b0930eb0f"
            }
          ]
        },
        {
          "id": "7a91000e-cc96-4099-bd56-6ce949b87f03",
          "name": "ListEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "919e9992-5e5b-4272-af4f-a420ebe93703"
            }
          ]
        },
        {
          "id": "f2b2e208-a69b-48fa-8799-bc0c66878d18",
          "name": "ListEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ba2eb80-69a7-441f-80e6-86ad5ef3f93b"
            }
          ]
        },
        {
          "id": "256b3442-06a4-4c85-85c6-ee3a00f76ac4",
          "name": "ListEvents1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroup/calendars/:id/events"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc7de698-3601-42dd-aebb-afa036753316"
            }
          ]
        },
        {
          "id": "10ae3611-adbe-4ae9-961c-00ee8d7c68e0",
          "name": "ListEvents1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroup/calendars/:id/events"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25ec3c6d-0fb3-4797-b928-b0c0f0fa21ee"
            }
          ]
        },
        {
          "id": "d3431819-a23c-4f61-acf3-0e0800fb50f0",
          "name": "ListEvents2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroups/:id/calendars/:id/events"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "117821a2-daae-4d55-acf7-04390866c401"
            }
          ]
        },
        {
          "id": "746eeec5-2f2a-4582-a4c4-fc58a1dcac0f",
          "name": "ListEvents2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroups/:id/calendars/:id/events"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29036b60-b21e-482e-a182-5d3fe445092c"
            }
          ]
        },
        {
          "id": "56918537-b7fc-4daf-a035-c8b0a8640d4b",
          "name": "ListCalendars",
          "request": {
            "url": "http://graph.microsoft.com/me/calendarGroup/calendars",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendars Retrieve a list of calendars belonging to a calendar group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e390d62-8edd-47c7-9312-def7d4a9c2fd"
            }
          ]
        },
        {
          "id": "c65c059d-87a8-4335-9f30-921e02fbf852",
          "name": "ListCalendars",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroup/calendars"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendars Retrieve a list of calendars belonging to a calendar group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb6916b7-25e3-424a-9251-f8deb52e2810"
            }
          ]
        },
        {
          "id": "4240f03c-8a6d-46b0-a4c5-46209b0df1c8",
          "name": "ListCalendars",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendarGroups/:id/calendars"
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
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendars Retrieve a list of calendars belonging to a calendar group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40f8e02f-dd43-49f0-a858-1bc7079360c9"
            }
          ]
        },
        {
          "id": "7f4d1aff-e121-49cd-8226-2d591a422439",
          "name": "ListCalendars",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendarGroups/:id/calendars"
              ],
              "variable": [
                {
                  "id": "id",
                  "v