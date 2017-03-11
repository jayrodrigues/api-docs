# List all exhibitors

This endpoint is to be retrieve a list of all exhibitors. where is_exhibitor = 1 in vendor table

## Resource

```
GET /exhibitors
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
              |      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/exhibitors'
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
      "id": 9,
      "company_id": 52,
      "description": null,
      "sponsor_level": 3,
      "location": null,
      "promotional_image": "",
      "attachments": "",
      "lead_retrieval": 1,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "44a24",
      "user_id": 8,
      "date_time": "1970-01-01 00:00:00",
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
      "id": 10,
      "company_id": 52,
      "description": null,
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
      "id": 11,
      "company_id": 52,
      "description": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": "",
      "attachments": "",
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "0bc26",
      "user_id": 10,
      "date_time": "1970-01-01 00:00:00",
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
      "id": 12,
      "company_id": 52,
      "description": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": "",
      "attachments": "",
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "79b10",
      "user_id": 10,
      "date_time": "1970-01-01 00:00:00",
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
      "id": 13,
      "company_id": null,
      "description": null,
      "sponsor_level": null,
      "location": null,
      "promotional_image": "",
      "attachments": "",
      "lead_retrieval": 0,
      "mobile_app_sponsor": 0,
      "is_exhibitor": 1,
      "access_code": "ab823",
      "user_id": 8,
      "date_time": "2017-03-11 22:19:15",
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
  "status_code": 200
}
```
### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
