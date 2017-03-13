# Get ads tracking details

This endpoint is to be retrieve all tracking of details of an ads

## Resource

```
GET /ads_tracking_details/{ads_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
ads_id | int| yes      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/ads_tracking_details/4'
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Activity details found",
  "status_code": 200,
  "data": {
    "data": [
      {
        "id": 1,
        "banner_id": 4,
        "type": "view",
        "datetime": "2017-03-13 09:48:39",
        "user_id": null
      }
    ],
    "count": 1,
    "banner_details": {
      "id": 4,
      "name": "Menu Ads update",
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
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

```json
{
  "message": "Ads not found",
  "status_code": 200,
}
```
