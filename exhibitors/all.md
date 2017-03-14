# List all exhibitors

This endpoint is to be retrieve a list of all exhibitors. where is_exhibitor = 1 in vendor table

## Resource

```
GET /{lang}/exhibitors
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
lang          | string     | yes | en/ar etc

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/en/exhibitors'
```

### Response

--------------------------------------------------------------------------------
Record found

ar

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
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
      "description": "Details in Ar",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    }
  ]
}
```

en

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
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
      "company_name": null
    }
  ]
}
```

Record Not found

**Status-Code:** `200 OK`

```json
{
  "message": "No record found",
  "status_code": 200,
  "data": []
}
```
### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
