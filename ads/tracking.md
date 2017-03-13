# Get current active ads based on ads type

This endpoint is to be retrieve one currently active ads by ads type.

## Resource

```
GET /ads/tracking/{ads_id}/{activity_type}
GET /ads/tracking/{ads_id}/{activity_type}/{user_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
activity_type | string| yes      | view,click
ads_id | int| yes      |

user_id | int| no      | user_id of current app user

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/ads/tracking/4/view'
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Activity added",
  "status_code": 200,
  "data": null
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

```json
{
  "message": "invalid activity type",
  "status_code": 400,
}
```
