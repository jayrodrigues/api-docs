# Users

This endpoint is to be used to update a user's profile.

## Resource

```
POST /auth/users/{id}
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :-----------------------------------------------------------------------------------
token         | string | yes      | Use the JWT token returned after successfully successfully logging into the account.
email         | string | yes      | Email address associated with the account.
first_name    | string | no       |
last_name     | string | no       |
phone         | string | no       |
zip           | string | no       |
address       | string | no       |
position      | string | no       |
google        | string | no       |
facebook      | string | no       |
linkedin      | string | no       |
twitter       | string | no       |
url           | string | no       |
instagram     | string | no       |
pinterest     | string | no       |
youtube       | string | no

## Example

### Request

--------------------------------------------------------------------------------

```
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `401 Could not decode token`

```json
{
  "message": "Could not decode token: The token \"eyJ0eXAiOiJKV1iLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjE3MiwiaXNzIjoiaHR0cDpcL1wvY29uZi1zdGcucHJvaHViLmlvXC9hcGlcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg4NjU5MjQ4LCJleHAiOjE0ODkwOTEyNDgsIm5iZiI6MTQ4ODY1OTI0OCwianRpIjoiMzk3NTFjNGQ0NWJmYWUwMTY5MjBjMGNkYTU0ZTI2MWUifQ.hQrXeXEnEhgflmRbfM0klQfLKS_q6Z-q4QfM-VajYhc\" is an invalid JWS",
  "status_code": 401,
}
```
