# Users

This endpoint will retrieve information about a user.

## Resource

```
POST /auth/users
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :-----------------------------------------------------------------------------------
token         | string | yes      | Use the JWT token returned after successfully logging into the account.

## Example

### Request

--------------------------------------------------------------------------------

```
curl -X GET "https://api.engageitapp.com/v1/monctonhomeshow2017/auth/users?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjE3MiwiaXNzIjoiaHR0cDpcL1wvY29uZi1zdGcucHJvaHViLmlvXC9hcGlcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg4NjU5MjQ4LCJleHAiOjE0ODkwOTEyNDgsIm5iZiI6MTQ4ODY1OTI0OCwianRpIjoiMzk3NTFjNGQ0NWJmYWUwMTY5MjBjMGNkYTU0ZTI2MWUifQ.hQrXeXEnEhgflmRbfM0klQfLKS_q6Z-q4QfM-VajYhc"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 172,
    "tieit_user_id": 224,
    "email": "test@test.com",
    "password": "$2y$08$0q0z6f8XkVoxFwGj1AnD4elTY/aASHAktrtuqM6AF96DywMcSuVWG",
    "company_id": 168,
    "active": 1,
    "first_name": "John Smith",
    "last_name": "",
    "city": "Toronto",
    "state": "Ontario",
    "country": "Canada",
    "phone": "",
    "avatar_file": "http://s3.amazon.com/uploads/profile_pics/b6e541f13ca5830373f0ad2681a41ba7.png",
    "zip": "",
    "address": "123 Sample Dr",
    "url": null,
    "about_me": "",
    "position": "Manager",
    "company_name": "Apple",
    "company_email": "est@test.com",
    "company_address": "123 Sample Dr",
    "company_description": null,
    "company_city": "Toronto",
    "company_state": "Ontario",
    "company_country": "Canada",
    "company_zip": "",
    "company_tel": "",
    "company_website": "",
    "social_media": [
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/facebook-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/twitter-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/google-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/youtube-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/pinterest-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/instagram-logo.png",
        "link": null
      },
      {
        "icon": "http://s3.amazon.com/uploads/social-media/png/linkedin-logo.png",
        "link": null
      }
    ]
  }
}
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
