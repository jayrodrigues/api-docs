# Get a Note

This endpoint is to be used to get details about a note.

## Resource

```
GET /notes/{note_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------------
note_id            | int  | yes      | ID of the note

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET "http://api.monctonhomeshow.engageitapp.com/v1/notes/1"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 1,
    "note": "Hello",
    "user_id": 8,
    "type": 1,
    "created_at": "2017-03-23 12:32:25",
    "updated_at": "2017-03-23 12:32:25",
    "is_active": 1,
    "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
    "first_name": "Meehdi",
    "last_name": "update",
    "email": "jay.rodrigues99@gmail.com"
  }
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
