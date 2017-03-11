# Update

This endpoint is to be used to update a track entry.

## Resource

```
POST /tracks/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the track

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
Updated successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Your changes have been saved successfully",
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
      "The title field is required."
    ]
  },
  "status_code": 422
}
```
