# Get a attendee details

This endpoint is to be retrieve details of a attendee by email.

## Resource

```
GET /attendees/details/{email}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | Yes

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/attendees/details/jay.rodrigues99@gmail.com'
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
    "first_name": "Jay",
    "last_name": "Rodrigues",
    "company_name": "Development Account",
    "company_email": "jay.rodrigues99@gmail.com",
    "company_phone": null
  }
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
