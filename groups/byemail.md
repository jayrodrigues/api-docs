# List all groups

This endpoint is to be retrieve a list of all groups for exhibitor synced from tieit.

## Resource

```
GET /groups/{user_id}/{email}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int     | yes
email       | string     | yes

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/groups/8/hasanmehdi89@gmail.com'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
      "id": 32,
      "tieit_group_id": 268,
      "name": "TestGroup1",
      "owner_id": 228,
      "company_id": 2,
      "is_public": 1,
      "added_date": "2017-03-11 19:07:20",
      "updated_date": null,
      "status": 1,
      "is_in_group": false
    },
    {
      "id": 31,
      "tieit_group_id": 271,
      "name": "GroupAdtN",
      "owner_id": 234,
      "company_id": 2,
      "is_public": 0,
      "added_date": "2017-03-11 19:07:20",
      "updated_date": null,
      "status": 1,
      "is_in_group": false
    },
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

**Status-Code:** ``

`json`
