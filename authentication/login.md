# Login

This endpoint is to be used to login for exhibitor with lead_retrieval yes only.

This endpoint will first try to login from local db if password not exist or can't login will try to login from tieit if succeed will sync user details, company details, Groups details from tieit to conf db.

## Resource

```
POST /auth/login
```

## Parameters

POST Parameter     | Type   | Required | Description
:---------------- | :----- | :------- | :----------------------------
email             | string | yes      |
password          | string | yes      |
unique_device_id  | string | yes      | given unique_device_id on new device creation.


## Example

### Request

--------------------------------------------------------------------------------

```
curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -d 'email=test@test.com&password=aeg@dfgesoihej&device_identifier=23443432432434332333333&device_type=1' "https://api.engageitapp.com/v1/monctonhomeshow2017/auth/login"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Login success",
  "status_code": 200,
  "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjE3MiwiaXNzIjoiaHR0cDpcL1wvY29uZi1zdGcucHJvaHViLmlvXC9hcGlcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg4NjU3MzczLCJleHAiOjE0ODkwODkzNzMsIm5iZiI6MTQ4ODY1NzM3MywianRpIjoiMDdhNzk4MzYyZGUzMmY3MzdjMWFlNDA4NzU0MTY1ZjkifQ.thIrXw8aPwFjw4iULdSudcDcqkuwCxxLrygsPOGrDcY"
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `300`

```json
{
  "message": "Email invalid or User not exists",
  "status_code": 300
}
```
