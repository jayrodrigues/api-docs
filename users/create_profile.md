# Create New User Profile

This endpoint is to be used to create new user profile (Without login details).

## Resource

```
POST /users/profile/{unique_device_id}
```

## Parameters
URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
unique_device_id| string  | yes      | unique id given on new device add by /add_this_device

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
email         | string | yes      | Email should be unique
first_name    | string | no       |
last_name     | string | no       |
company       | int    | no       | company id
city          | string | no       |
state         | string | no       |
country       | string | no       |
phone         | string | no       |
avatar_file   | file   | no       | profile picture
zip           | string | no       |
address       | string | no       |
linkedin      | string | no       |
twitter       | string | no       |
url           | string | no       |
company_email | string | no       |
facebook      | string | no       |
instagram     | string | no       |
pinterest     | string | no       |
youtube       | string | no       |
google        | string | no       |
about_me      | text   | no       |
bio           | text   | no       |
position      | string | no       |
is_speaker    | int    | no       | 0=no,1=yes. default 0. set value as 1 to mark as speaker
is_public     | int    | no       | 0=no,1=yes. default 1. if public will return all data in user details response
user_type     | int    | no       | 1=admin,2=exhibitor,3=attendee. default 3

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl ''
```

### Response

--------------------------------------------------------------------------------
Created successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "email": "hasanmehdi89+1@gmail.com",
    "avatar_file": "",
    "id": 8
    ....
  }
}
```

### Error Responses

--------------------------------------------------------------------------------
Validation Error

**Status-Code:** `422 Unprocessable Entity`

```json
{
  "message": "Can't create new record",
  "errors": {
    "title": [
      "The email field is required."
    ]
  },
  "status_code": 422
}
```
```json
{
  "message": "Can't create new record",
  "errors": {
    "email": [
      "The email has already been taken."
    ]
  },
  "status_code": 422
}
```

Can't upload attachments

**Status-Code:** `500 Internal Server Error`

```json
{
  "message": "The target directory `uploads/profile_pics` does not exists or is not writable",
  "status_code": 500
}
```

Unsupported Media Type

**Status-Code:** `415 Unsupported Media Type`

```json
{
  "message": "Please upload a valid file (png/jpeg/gif)",
  "status_code": 415
}
```
