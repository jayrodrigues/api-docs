# Create Note

This endpoint is to be used to create a note entry.

## Resource

```
POST /notes
```

## Parameters

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
note | text | yes |
type | int | yes |
user_id | int | yes | current user crating this note


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
    "type": "1",
    "user_id": "8",
    "updated_at": "2017-03-23 12:32:25",
    "created_at": "2017-03-23 12:32:25",
    "id": 1
  }
}
```

### Error Responses

--------------------------------------------------------------------------------
