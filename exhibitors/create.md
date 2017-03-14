# Create Exhibitors

This endpoint is to be used to create new exhibitor by admin. This endpoint will create exhibitor and also create a user with that email address then will send a special code to used email. So, that exhibitor can use that code to login and sync there tieit data into conf app

login required. request with JWT token in header
## Resource

```
POST /exhibitors
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
email         | string | yes      |
lang         | string | yes      | en/es etc
lead_retrieval| int    | yes      | 0-no, 1-yes
mobile_app_sponsor| int| yes      | 0-no, 1-yes
promotional_image| file | no      |
attachments   | file   | no       |
is_exhibitor  | int    | no       |
company_id    | int    | no       |
description   | text | yes       |
sponsor_level | int    | no       | 1 Platinum, 2 Emerald, 3 Gold, 4 Silver, 5 Pearl, 6 Bronze
location      | string | no       |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl ''
```

### Response

--------------------------------------------------------------------------------
Created successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "promotional_image": "",
    "attachments": "",
    "date_time": 1489270595,
    "is_exhibitor": 1,
    "company_id": null,
    "description": null,
    "sponsor_level": null,
    "location": null,
    "access_code": "ab823",
    "user_id": 8,
    "id": 13
  }
}
```

### Error Responses

--------------------------------------------------------------------------------
Validation Error

**Status-Code:** `422 Unprocessable Entity`

```json
{
  "message": "Can't create new record",
  "errors": {
    "title": [
      "The email field is required."
    ]
  },
  "status_code": 422
}
```

Can't upload attachments

**Status-Code:** `500 Internal Server Error`

```json
{
  "message": "The target directory `uploads/exhibitors` does not exists or is not writable",
  "status_code": 500
}
```

Unsupported Media Type

**Status-Code:** `415 Unsupported Media Type`

```json
{
  "message": "Please upload a valid file (png/jpeg/gif)",
  "status_code": 415
}
```
