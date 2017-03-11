# Get Contact Details

This endpoint will retrieve information about a contact by email.

## Resource

```
POST /get_contact_details/{user_id}
```

## Parameters

URI Parameter | Type   | Required | Description
:------------ | :----- | :------- | :-----------------------------------------------------------------------------------
user_id       | string | yes      | User ID to get details

POST Parameter | Type   | Required | Description
:------------  | :----- | :------- | :-----------------------------------------------------------------------------------
email          | string | yes      |


## Example

### Request

--------------------------------------------------------------------------------

```
curl ""
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
    "contact_email": "jay.rodrigues99@gmail.com",
    "first_name": "Jay",
    "last_name": "Rodrigues",
    "city": "Toronto",
    "state": "Ontario",
    "country": "Canada",
    "phone": null,
    "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/f43786ea4629036e22fffbc3567b6777.jpg",
    "zip": "",
    "address": "123 Sample Dr",
    "facebook": null,
    "instagram": null,
    "pinterest": null,
    "youtube": null,
    "google": null,
    "twitter": null,
    "linkedin": null,
    "url": null,
    "about_me": null,
    "position": null,
    "bio": null,
    "company_name": "Development Account",
    "company_email": "jay.rodrigues99@gmail.com",
    "company_address": "123 Sample Dr",
    "company_address2": "123 Sample Dr",
    "company_description": null,
    "company_city": "Toronto",
    "company_state": "Ontario",
    "company_country": "Canada",
    "company_zip": "",
    "company_tel": null,
    "company_website": "",
    "connected_contact": 0
  }
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `401 Could not decode token`

```json
{
  "message": "Valdiation failed",
  "errors": {
    "email": [
      "The email field is required."
    ]
  },
  "status_code": 422,
}
```
