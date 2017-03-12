# Get single Session

This endpoint is to be retrieve one session details by session id.

## Resource

```
GET /sessions/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the session

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/sessions/1'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 1,
    "title": "Test sessions 2",
    "survey_url": "https://github.com",
    "abstract": "Little info about session",
    "track_title": "Marketing update",
    "location": "center hall",
    "attachments": "",
    "session_date": "2017-03-09",
    "start_time": "00:00:00",
    "speaker_id": 8,
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
  }
}
```

Record Not found (If given session id not exists in database)

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
