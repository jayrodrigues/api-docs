# Create New Ads

This endpoint is to create new Ads of any type

Login required and only admin can create ads

## Resource

```
POST /ads
```

## Parameters

POST Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
name      | string  | yes      |
type      | int  | yes      | 1-menu,2-banner,3-splash
image      | file  | no      |
image_url      | string  | no      |
button_text      | string  | no      |
button_url      | string  | no      |
company_id      | int  | no      | Must exist in company table

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X POST 'http://api.monctonhomeshow.engageitapp.com/v1/ads'
```

### Response

--------------------------------------------------------------------------------
**Status-Code:** `200 OK`

```json
{
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "name": "Menu Ads",
    "type": "1",
    "image": "",
    "user_id": 8,
    "is_active": 1,
    "added_date": "2017-03-13 09-22-02",
    "id": 6
  }
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``
```json
{
  "message": "Could not create.",
  "errors": {
    "name": [
      "The name field is required."
    ],
    "type": [
      "The type field is required."
    ]
  },
  "status_code": 422,
}
```

```json
{
  "message": "Could not create.",
  "errors": {
    "company_id": [
      "The selected company id is invalid."
    ]
  },
  "status_code": 422,
}
```


```json
{
  "message": "The token could not be parsed from the request",
  "status_code": 500,
}
```

```json
{
  "message": "Only admin can perform this operation",
  "status_code": 400,
  "data": null
}
```
