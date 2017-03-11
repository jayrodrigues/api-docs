# retrieve special login code by email

This endpoint is to be retrieve special login code by email.

## Resource

```
GET /exhibitors/retrieve_code/{email}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
email         | int  | yes      | exhibitor email

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/exhibitors/retrieve_code/hasanmehdi89@gmail.com'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Code sent successfully to exhibitor",
  "status_code": 200,
}
```

Record Not found

**Status-Code:** `200 OK`

```json
{
  "message": "Email not valid or exists",
  "status_code": 400,
}
```
### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** ``

`json`
