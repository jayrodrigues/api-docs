# Create New User Profile

This endpoint is to be used to create new user profile (Without login details).

## Resource

```
POST /user/create_profile
```

## Parameters

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
  "message": "Your changes have been updated successfully",
  "status_code": 200
}
```

### Error Responses

--------------------------------------------------------------------------------
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