# List all attendees

This endpoint is to be retrieve a list of all attendees.

## Resource

```
GET /attendees/{user_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
              |      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/sessions'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
      "user_id": 8,
      "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
      "about_me": null,
      "email": "jay.rodrigues99@gmail.com",
      "first_name": "Jay",
      "last_name": "Rodrigues",
      "position": null,
      "connected_contacts": null,
      "contact_link_id": null,
      "company_name": "Development Account",
      "company_address": "123 Sample Dr",
      "company_phone": null,
      "company_email": "jay.rodrigues99@gmail.com",
      "company_city": "Toronto",
      "company_state": "Ontario"
    },
    {
      "user_id": 10,
      "avatar_file": "",
      "about_me": null,
      "email": "hasanmehdi89@gmail.com",
      "first_name": null,
      "last_name": null,
      "position": null,
      "connected_contacts": null,
      "contact_link_id": null,
      "company_name": null,
      "company_address": null,
      "company_phone": null,
      "company_email": null,
      "company_city": null,
      "company_state": null
    },
    {
      "user_id": 11,
      "avatar_file": "",
      "about_me": null,
      "email": "hasanmehdi89+1@gmail.com",
      "first_name": null,
      "last_name": null,
      "position": null,
      "connected_contacts": 1,
      "contact_link_id": 7,
      "company_name": null,
      "company_address": null,
      "company_phone": null,
      "company_email": null,
      "company_city": null,
      "company_state": null
    }
  ]
}
```

Record Not found

**Status-Code:** `200 OK`

```json
{
  "message": "No record found",
  "status_code": 200
}
```
### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
