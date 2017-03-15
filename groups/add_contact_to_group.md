# Add Contact into a group and sync back to tieit

Add already linked contact into one or multiple group

## Resource

```
POST /groups/add
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
email       | string     | yes | who you want to add to group
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
  "message": "Created successfully",
  "status_code": 200,
  "data": [
    {
      "contact_id": 12,
      "group_id": "32",
      "added_date": "2017-03-15 15-47-25",
      "id": 5
    }
  ]
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

```json
{
  "message": "Contact already exists with this group",
  "status_code": 200,
}
```
