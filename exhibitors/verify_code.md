# verify access code for exhibitors to display login

This endpoint is to be verify exhibitors access code.

## Resource

```
GET /exhibitors/verify/{email}/{access_code}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
email         | int  | yes      | exhibitor email
access_code   | string| yes      | on new exhibitor create by admin we send an access_code to given email. use that access code here

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET 'http://api.monctonhomeshow.engageitapp.com/v1/exhibitors/retrieve_code/hasanmehdi89@gmail.com/79b10'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Code verified",
  "status_code": 200,
}
```

### Error Responses

--------------------------------------------------------------------------------
**Status-Code:** `400 error`

```json
{
  "message": "Code not valid",
  "status_code": 400,
}
```
