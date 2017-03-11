# List all Sessions

This endpoint is to be retrieve a list of all sessions.

## Resource

```
GET /sessions
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
      "id": 1,
      "title": "Test sessions",
      "survey_url": null,
      "abstract": "",
      "track_id": null,
      "speaker_id": null,
      "duration": 0,
      "location": "",
      "attachments": "",
      "description": null,
      "end_time": null,
      "session_date": "0000-00-00",
      "start_time": "00:00:00",
      "date_time": 1489242062,
      "track_title": null,
      "speaker_name": null
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
