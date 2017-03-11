# Create Sessions

This endpoint is to be used to create a session entry.

## Resource

```
POST /speakers
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
title         | string | yes      |
abstract      | string | no       |
description   | string | no       |
track_id      | string | no       |
speaker_id    | string | no       |
duration      | string | no       |
location      | string | no       |
attachments   | file   | no       |
session_date  | date   | no       |
start_time    |        | no       |
end_time      |        | no       |
survey_url    | url    | no

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'sdfdfsdf'
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Session created",
  "status_code": 200,
  "data": [
    {
      "id": 1,
      "title": "Exhibitor Move-In",
      "survey_url": null,
      "abstract": "",
      "track_id": 0,
      "speaker_id": 0,
      "duration": 240,
      "location": "Palms A-E",
      "attachments": "",
      "description": null,
      "end_time": "20:00:00",
      "session_date": "2016-11-13",
      "start_time": "16:00:00",
      "date_time": 1476827316,
      "track_title": null,
      "speaker_name": null
    }
]
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `400 Title Required`

```json
{
    "": ""
}
```
