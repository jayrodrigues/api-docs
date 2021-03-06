# update Exhibitors data only

This endpoint is to be used to update exhibitor(vendor) table data only

login required. request with JWT token in header
## Resource

```
POST /exhibitors
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
lead_retrieval| int    | no      | 0-no, 1-yes
lang          | string | yes      | en/es etc
mobile_app_sponsor| int| no      | 0-no, 1-yes
promotional_image| file | no      |
attachments   | file   | no       |
is_exhibitor  | int    | no       |
company_id    | int    | no       |
description   | string | no       |
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
  "message": "Your changes have been updated successfully",
  "status_code": 200,
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
