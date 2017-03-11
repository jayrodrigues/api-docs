# Create

This endpoint is to be used to create a track entry.

## Resource

```
POST /tracks
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
title         | string | yes      |
description   | text   | yes      |

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
    "title": "Marketing",
    "description": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
    "date_time": 1489250259,
    "id": 1
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
      "The title field is required."
    ]
  },
  "status_code": 422
}
```
