# Get current active ads based on ads type

This endpoint is to be retrieve one currently active ads by ads type.

## Resource

```
GET /ads/{ads_type}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
ads_type      | string  | yes      | 1-menu,2-banner,3-splash

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/ads/menu'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Current ads found",
  "status_code": 200,
  "data": {
    "id": 4,
    "name": "Menu Ads 2",
    "image": null,
    "image_url": null,
    "is_current": 1,
    "user_id": 8,
    "button_text": "AWESOME",
    "button_url": null,
    "company_id": 1,
    "type": 1,
    "is_active": 1,
    "added_date": null,
    "schedule_date": "2017-03-13 03:00:00",
    "company_name": null,
    "company_city": null,
    "company_address": null
  }
}
```

Record Not found

**Status-Code:** `200 OK`

```json
{
  "message": "ads not found",
  "status_code": 200,
}
```
### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
