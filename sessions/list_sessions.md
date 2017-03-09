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

````curl
curl -X GET "https://api.engageitapp.com/monctonhomeshow2017/sessions"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
    "message": "Data found",
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
        },
        {
            "id": 2,
            "title": "Registration",
            "survey_url": "",
            "abstract": "",
            "track_id": 0,
            "speaker_id": 0,
            "duration": 120,
            "location": "Palms Foyer",
            "attachments": "",
            "description": null,
            "end_time": "21:00:00",
            "session_date": "2016-11-13",
            "start_time": "18:00:00",
            "date_time": 1475842072,
            "track_title": null,
            "speaker_name": null
        },
        {
            "id": 19,
            "title": "Broker Meet & Greet ",
            "survey_url": "",
            "abstract": "Sponsored by Vend Tech International",
            "track_id": 0,
            "speaker_id": 0,
            "duration": 180,
            "location": "Palms Foyer",
            "attachments": "",
            "description": "",
            "end_time": "21:00:00",
            "session_date": "2016-11-13",
            "start_time": "18:00:00",
            "date_time": 1475842072,
            "track_title": null,
            "speaker_name": null
        },        
        {
            "id": 72,
            "title": "Break",
            "survey_url": null,
            "abstract": "",
            "track_id": null,
            "speaker_id": null,
            "duration": 10,
            "location": "",
            "attachments": "",
            "description": null,
            "end_time": "10:00:00",
            "session_date": "2016-11-16",
            "start_time": "09:50:00",
            "date_time": 1476828677,
            "track_title": null,
            "speaker_name": null
        }
    ]
}
````

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
