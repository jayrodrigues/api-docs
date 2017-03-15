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
      "id": 16,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": null,
      "attachments": null,
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "3011",
      "user_id": 10,
      "date_time": "2017-03-14 12:32:39",
      "description": "Exhibitor Description",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 17,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": null,
      "attachments": null,
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "ab05",
      "user_id": 10,
      "date_time": "2017-03-14 12:32:52",
      "description": "Exhibitor Description",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 18,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": null,
      "attachments": null,
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "42d2",
      "user_id": 10,
      "date_time": "2017-03-14 12:34:11",
      "description": "Exhibitor Description",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 19,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": null,
      "attachments": null,
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "121d",
      "user_id": 10,
      "date_time": "2017-03-14 12:37:46",
      "description": "Exhibitor Description",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 20,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": "https://api.monctonhomeshow.engageitapp.com/uploads/vendors/promotional_image/e762bf01525d5462b3002e606887c1e3.png",
      "attachments": "https://api.monctonhomeshow.engageitapp.com/uploads/vendors/attachments/e762bf01525d5462b3002e606887c1e3.pdf",
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "b02a",
      "user_id": 10,
      "date_time": "2017-03-14 12:50:01",
      "description": "Exhibitor Description",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 21,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": "https://api.monctonhomeshow.engageitapp.com/uploads/vendors/promotional_image/ec9b0f7b4a33595b74f5fdc835c364cb.png",
      "attachments": "https://api.monctonhomeshow.engageitapp.com/uploads/vendors/attachments/ec9b0f7b4a33595b74f5fdc835c364cb.pdf",
      "lead_retrieval": 1,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "ee36",
      "user_id": 8,
      "date_time": "2017-03-14 12:51:01",
      "description": "Exhibitor Description for jay user",
      "lang": "en",
      "sm_twitter": null,
      "sm_facebook": null,
      "sm_google": null,
      "sm_instagram": null,
      "company_website": null,
      "company_phone": null,
      "comapny_email": null,
      "comapny_logo": null,
      "company_name": null
    },
    {
      "id": 22,
      "company_id": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": null,
      "attachments": null,
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "acc1",
      "user_id": 8,
      "date_time": "2017-03-14 21:39:56",
      "description": "Exhibitor Null test",
      "lang": "en",
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
