# Get single exhibitor

This endpoint is to be retrieve one exhibitor details by exhibitor id.

## Resource

```
GET /exhibitors/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the exhibitor
lang          | string     | yes | en/ar etc

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/en/exhibitors/1'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 10,
    "company_id": 52,
    "sponsor_level": null,
    "location": null,
    "promotional_image": "",
    "attachments": "",
    "lead_retrieval": 0,
    "mobile_app_sponsor": 0,
    "is_exhibitor": 1,
    "access_code": "f9a2a",
    "user_id": 10,
    "date_time": "1970-01-01 00:00:00",
    "description": "Details in en",
    "sm_twitter": null,
    "sm_facebook": null,
    "sm_google": null,
    "sm_instagram": null,
    "company_website": null,
    "company_phone": null,
    "comapny_email": null,
    "comapny_logo": null,
    "company_name": null,
    "users": []
  }
}
```

Record Not found (If given session id not exists in database)

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
