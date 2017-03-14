# Set current active ads based on ads type and ads id

This endpoint is to set current active ads by ads type and ads id.

login required and only admin can perform this

## Resource

```
GET /ads/{ads_type}/{ads_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
ads_type      | string  | yes      | 1-menu,2-banner,3-splash
ads_id      | int  | yes      | ID of ads

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/ads/menu/4'
```

### Response

--------------------------------------------------------------------------------
set successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Activated as current ads successfully",
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
    "schedule_date": "2017-03-13 03:00:00"
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

```json
{
  "message": "Only admin can perform this operation",
  "status_code": 400,
  "data": null
}
```
