# Create Speaker

This endpoint is to be used to update a speaker entry.

Login required
## Resource

```
POST /notes/{note_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------------
note_id            | int  | yes      | ID of the note

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
note | text | yes |
user_id | int | yes | current user crating this note
is_active|int| no|



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
  "message": "Your changes have been saved successfully",
  "status_code": 200,
}
```

### Error Responses

--------------------------------------------------------------------------------
