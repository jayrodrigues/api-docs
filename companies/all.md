# List all companies

This endpoint is to be retrieve a list of all companies.

## Resource

```
GET /companies
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
              |      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/companies'
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
      "date_time": "2017-03-11 19:07:18"
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
