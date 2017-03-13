# Users

This endpoint will retrieve information about a user.

## Resource

```
GET /users/{user_id}
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :-----------------------------------------------------------------------------------
user_id       | string | yes      | User ID to get details

## Example

### Request

--------------------------------------------------------------------------------

```
curl -X GET "https://api.engageitapp.com/v1/monctonhomeshow2017/auth/users?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjE3MiwiaXNzIjoiaHR0cDpcL1wvY29uZi1zdGcucHJvaHViLmlvXC9hcGlcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg4NjU5MjQ4LCJleHAiOjE0ODkwOTEyNDgsIm5iZiI6MTQ4ODY1OTI0OCwianRpIjoiMzk3NTFjNGQ0NWJmYWUwMTY5MjBjMGNkYTU0ZTI2MWUifQ.hQrXeXEnEhgflmRbfM0klQfLKS_q6Z-q4QfM-VajYhc"
```

### Response

--------------------------------------------------------------------------------

If is_public = 1

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 10,
    "tieit_user_id": null,
    "email": "hasanmehdi89@gmail.com",
    "password": null,
    "company_id": null,
    "active": 1,
    "first_name": null,
    "last_name": null,
    "city": null,
    "state": null,
    "country": null,
    "phone": null,
    "avatar_file": "",
    "zip": null,
    "address": null,
    "is_public": 1,
    "url": null,
    "about_me": null,
    "position": null,
    "company_name": null,
    "company_email": null,
    "company_address": null,
    "company_description": null,
    "company_city": null,
    "company_state": null,
    "company_country": null,
    "company_zip": null,
    "company_tel": null,
    "company_website": null,
    "is_exhibitor": 1,
    "lead_retrieval": 0,
    "exhibitor_id": 10,
    "social_media": [
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/facebook-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/twitter-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/google-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/youtube-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/pinterest-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/instagram-logo.png",
        "link": null
      },
      {
        "icon": "http://awesome.dev/engageitapimoncton/public/uploads/social-media/png/linkedin-logo.png",
        "link": null
      }
    ]
  }
}
```

If is_public = 0

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "first_name": "Jay",
    "last_name": "Rodrigues",
    "company_name": "Development Account",
    "company_id": 2,
    "id": 8,
    "is_public": 0
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
