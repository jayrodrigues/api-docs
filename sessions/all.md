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
      "title": "Test sessions 2",
      "survey_url": "https://github.com",
      "abstract": "Little info about session",
      "track_id": 1,
      "speaker_id": 8,
      "duration": 0,
      "location": "center hall",
      "attachments": "",
      "description": null,
      "end_time": "00:00:00",
      "session_date": "2017-03-09",
      "start_time": "00:00:00",
      "date_time": 1489242062,
      "track_title": "Marketing update",
      "speaker_data": [
        {
          "user_id": 8,
          "first_name": "Jay",
          "last_name": "Rodrigues",
          "email": "jay.rodrigues99@gmail.com",
          "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
          "company_name": null
        }
      ]
    },
    {
      "id": 3,
      "title": "Test sessions 2",
      "survey_url": "https://github.com",
      "abstract": "Little info about session",
      "track_id": 1,
      "speaker_id": 8,
      "duration": 0,
      "location": "center hall",
      "attachments": "",
      "description": null,
      "end_time": "00:00:00",
      "session_date": "2017-03-09",
      "start_time": "02:08:00",
      "date_time": 1489242853,
      "track_title": "Marketing update",
      "speaker_data": [
        {
          "user_id": 8,
          "first_name": "Jay",
          "last_name": "Rodrigues",
          "email": "jay.rodrigues99@gmail.com",
          "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
          "company_name": null
        }
      ]
    },
    {
      "id": 4,
      "title": "Marketing",
      "survey_url": null,
      "abstract": "",
      "track_id": null,
      "speaker_id": null,
      "duration": 0,
      "location": "",
      "attachments": "",
      "description": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
      "end_time": null,
      "session_date": "0000-00-00",
      "start_time": "00:00:00",
      "date_time": 1489249821,
      "track_title": null,
      "speaker_data": []
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
