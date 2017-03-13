# List all ads

This endpoint is to be retrieve a list of all ads.

## Resource

```
GET /ads
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
              |      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/ads'
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
      "id": 1,
      "name": "Menu Ads",
      "image": null,
      "image_url": null,
      "is_current": 0,
      "user_id": 8,
      "button_text": "AWESOME",
      "button_url": null,
      "company_id": 1,
      "type": 1,
      "is_active": 1,
      "added_date": null,
      "schedule_date": "2017-03-13 03:00:00"
    },
    {
      "id": 2,
      "name": "Banner ads",
      "image": null,
      "image_url": null,
      "is_current": 0,
      "user_id": 8,
      "button_text": "AWESOME",
      "button_url": null,
      "company_id": 1,
      "type": 2,
      "is_active": 1,
      "added_date": null,
      "schedule_date": "2017-03-13 03:00:00"
    },
    {
      "id": 3,
      "name": "Splash ads",
      "image": null,
      "image_url": null,
      "is_current": 1,
      "user_id": 8,
      "button_text": "AWESOME",
      "button_url": null,
      "company_id": 1,
      "type": 3,
      "is_active": 1,
      "added_date": null,
      "schedule_date": "2017-03-13 03:00:00"
    },
    {
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
    },
    {
      "id": 5,
      "name": "Banner ads 2",
      "image": null,
      "image_url": null,
      "is_current": 1,
      "user_id": 8,
      "button_text": "AWESOME",
      "button_url": null,
      "company_id": 1,
      "type": 2,
      "is_active": 1,
      "added_date": null,
      "schedule_date": "2017-03-13 03:00:00"
    }
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
