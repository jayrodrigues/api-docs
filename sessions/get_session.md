# Get Detail about a specific Session

This endpoint is to be retrieve information about a specific session.

## Resource

```
GET /sessions/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------------
id            | int  | yes      | ID of the session

## Example

### Request

--------------------------------------------------------------------------------

````curl
curl -X GET "https://api.engageitapp.com/monctonhomeshow2017/sessions/12"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 2,
    "title": "Registration",
    "survey_url": "",
    "abstract": "",
    "track_title": null,
    "location": "Palms Foyer",
    "attachments": "",
    "session_date": "2016-11-13",
    "start_time": "18:00:00",
    "speaker_id": null,
    "speaker_name": null,
    "speaker_picture": null,
    "speaker_company": null
  }
}
````

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
