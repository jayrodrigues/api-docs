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
    "title": "Test sessions",
    "survey_url": null,
    "abstract": "",
    "track_title": null,
    "location": "",
    "attachments": "",
    "session_date": "0000-00-00",
    "start_time": "00:00:00",
    "speaker_id": null,
    "speaker_name": null,
    "speaker_picture": null,
    "speaker_company": null
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
