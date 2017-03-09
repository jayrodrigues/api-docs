# Groups

The registration endpoint is used to login into existing user accounts.

## Resource

```
POST /auth/login
```

## Parameters

URI Parameter     | Type   | Required | Description
:---------------- | :----- | :------- | :----------------------------
email             | string | yes      |
password          | string | yes      |
device_identifier | string | no       |
device_type       | int    | no       | 0 = iOS; 1 = Android (verify)
device_os         | string | no       | remove from db
device_model      | string | no       | remove from db

## Example

### Request

--------------------------------------------------------------------------------

```
curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -d 'email=test@test.com&password=aeg@dfgesoihej' "https://api.engageitapp.com/v1/monctonhomeshow2017/auth/login"
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
