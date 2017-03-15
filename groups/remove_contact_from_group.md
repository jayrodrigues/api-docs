# Remove Contact from a group and sync back to tieit

## Resource

```
POST /groups/remove
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
contact_id       | int     | yes | user_contact table id
group_id       | int     | yes

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
  "message": "Removed contact from group successfully",
  "status_code": "200",
  "data": null
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

```json
{
  "message": "No data found to remove",
  "status_code": 400,
}
```
