# Get all notes of given user

This endpoint is to be used to get all notes of a User

## Resource

```
GET /users/notes/{owner_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------------
owner_id            | int  | yes      | exhibitor user_id

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET "http://api.monctonhomeshow.engageitapp.com/v1/users/notes/1"
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
      "note": "Hello update",
      "user_id": 8,
      "owner_id": 1,
      "type": 1,
      "created_at": "2017-03-23 12:51:33",
      "updated_at": "2017-03-23 12:51:33",
      "is_active": 1,
      "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
      "first_name": "Meehdi",
      "last_name": "hello",
      "email": "jay.rodrigues99@gmail.com"
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
