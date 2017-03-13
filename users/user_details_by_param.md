# Users details

This endpoint will retrieve information about a user by unique_device_id and email.

## Resource

```
GET /users/{unique_device_id}/{email}
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :-----------------------------------------------------------------------------------
unique_device_id       | string | yes      | On device add generated unique_device_id
email       | string | yes      | User email used to create profile

## Example

### Request

--------------------------------------------------------------------------------

```
curl -X GET "http://awesome.dev/engageitapimoncton/public/api/v1/users/f1af518194ed957/jay.rodrigues99@gmail.com"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 8,
    "tieit_user_id": 224,
    "email": "jay.rodrigues99@gmail.com",
    "company_id": 2,
    "active": 1,
    "first_name": "Jay",
    "last_name": "Rodrigues",
    "city": "Toronto",
    "state": "Ontario",
    "country": "Canada",
    "phone": null,
    "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
    "zip": "",
    "address": "123 Sample Dr",
    "url": null,
    "about_me": null,
    "position": null,
    "company_name": "Development Account",
    "company_email": "jay.rodrigues99@gmail.com",
    "company_address": "123 Sample Dr",
    "company_description": null,
    "company_city": "Toronto",
    "company_state": "Ontario",
    "company_country": "Canada",
    "company_zip": "",
    "company_tel": null,
    "company_website": "",
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

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `400`

```json
{
  "message": "Users not exists or not found",
  "status_code": 400,
}
```
