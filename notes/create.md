# Create Note

This endpoint is to be used to create a note entry.

Login required
## Resource

```
POST /notes
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
note | text | yes |
user_id | int | yes | current user crating this note
is_active|int| no| default 1

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl ''
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "note": "Hello",
    "user_id": "8",
    "updated_at": "2017-03-23 12:32:25",
    "created_at": "2017-03-23 12:32:25",
    "id": 1
  }
}
```

### Error Responses

--------------------------------------------------------------------------------
