# Add Contact into a group and sync back to tieit

## Resource

```
POST /add_contact_to_group
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
