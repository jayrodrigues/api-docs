# Update Ads

This endpoint is to Update Ads of any type

Login required and only admin can perform this operation

## Resource

```
POST /ads/{ads_id}
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
curl -X POST 'http://api.monctonhomeshow.engageitapp.com/v1/ads/4'
```

### Response

--------------------------------------------------------------------------------
**Status-Code:** `200 OK`

```json
{
  "message": "updated successfully",
  "status_code": 200,
  "data": null
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
  "message": "No data found to update",
  "status_code": 400,
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
