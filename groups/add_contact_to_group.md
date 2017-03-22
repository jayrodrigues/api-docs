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
group_id       | int     | yes | can be passed multiple group id with , like 20,21,22

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
      "contact_id": 16,
      "group_id": "20",
      "added_date": "2017-03-22 16-34-19",
      "id": 15
    },
    {
      "contact_id": 16,
      "group_id": "21",
      "added_date": "2017-03-22 16-34-21",
      "id": 16
    },
    {
      "contact_id": 16,
      "group_id": "22",
      "added_date": "2017-03-22 16-34-22",
      "id": 17
    }
  ]
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

```json
{
  "message": "Contact already exists with these groups[\"20\",\"21\",\"22\"]",
  "status_code": 400,
}
```

```json
{
  "message": "Your given group id 5646 is not exits",
  "status_code": 422,
}
```
