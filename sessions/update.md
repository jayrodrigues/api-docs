# Update Sessions

This endpoint is to be used to update a session entry.

## Resource

```
POST /sessions/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the session

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
title         | string | yes      |
speaker_id    | int    | yes      | Given ID Should exists as speaker
track_id      | int    | no       | Tracks table id
session_date  | date   | no       | 2017-03-09
start_time    | time   | no       | 02:08:00
end_time      | time   | no       | 05:08:00
location      | string | no       |
abstract      | string | no       |
survey_url    | string | no       |
attachments   | file   | no       |

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
  "status_code": 200
}
```

### Error Responses

--------------------------------------------------------------------------------
Validation Error

**Status-Code:** `422 Unprocessable Entity`

```json
{
  "message": "Can't update record",
  "errors": {
    "title": [
      "The title field is required."
    ]
  },
  "status_code": 422
}
```

Can't upload attachments

**Status-Code:** `500 Internal Server Error`

```json
{
  "message": "The target directory `uploads/sessions` does not exists or is not writable",
  "status_code": 500
}
```

Unsupported Media Type

**Status-Code:** `415 Unsupported Media Type`

```json
{
  "message": "Please upload a valid file (pdf/doc/xlxs/xls/csv/png/jpeg/gif)",
  "status_code": 415
}
```
