# Get single company

This endpoint is to be retrieve one company details by company id.

## Resource

```
GET /companies/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the company

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/companies/1'
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
    "id": 2,
    "tieit_company_id": 52,
    "company_name": "Development Account",
    "description": null,
    "address": "123 Sample Dr",
    "address_line2": "123 Sample Dr",
    "picture": "",
    "city": "Toronto",
    "state": "Ontario",
    "country": "Canada",
    "zip": "",
    "tel": null,
    "email": "jay.rodrigues99@gmail.com",
    "website": "",
    "sm_twitter": null,
    "sm_google": null,
    "sm_facebook": null,
    "sm_instagram": null,
    "category_id": null,
    "date_time": 1489259238
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
