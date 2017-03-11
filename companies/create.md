# Create Company

This endpoint is to be used to create new company

login required. request with JWT token in header
## Resource

```
POST /companies
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
company_name         | string | yes      |
description         | string | no      |
address         | string | no      |
address_line2         | string | no      |
picture         | file | no      |
city         | string | no      |
state         | string | no      |
country         | string | no      |
zip         | string | no      |
tel         | string | no      |
email         | string | no      |
website         | string | no      |
sm_twitter         | string | no      |
sm_facebook         | string | no      |
sm_google         | string | no      |
sm_instagram         | string | no      |
category_id         | string | no      | from category table


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
    "company_name": "Ackosoft",
    "date_time": 1489271414,
    "picture": "",
    "id": 3
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
    "company_name": [
      "The company name field is required."
    ]
  },
  "status_code": 422,
}
```

Can't upload attachments

**Status-Code:** `500 Internal Server Error`

```json
{
  "message": "The target directory `uploads/companies` does not exists or is not writable",
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
