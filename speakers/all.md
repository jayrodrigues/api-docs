# Get All Speakers

This endpoint is to be used to get a list of all Speakers.

## Resource

```
GET /speakers
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
              |      |

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET "http://api.monctonhomeshow.engageitapp.com/v1/speakers"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

Record Found

```json
{
    "message": "Data found",
    "status_code": 200,
    "data": [
        {
            "id": 1,
            "company_id": null,
            "first_name": "Douglas",
            "last_name": "Alvarez",
            "title": null,
            "bio": null,
            "about_me": null,
            "company_name": null,
            "twitter": null,
            "google": null,
            "facebook": null,
            "instagram": null,
            "avatar_file": "",
            "phone": null,
            "url": null
        },
        {
            "id": 2,
            "company_id": null,
            "first_name": "Claire",
            "last_name": "Fowler",
            "title": null,
            "bio": null,
            "about_me": null,
            "company_name": null,
            "twitter": null,
            "google": null,
            "facebook": null,
            "instagram": null,
            "avatar_file": "",
            "phone": "111-111-1111",
            "url": null
        }
    ]
}
```


Record Not found

**Status-Code:** `200 OK`

```json
{
  "message": "No record found",
  "status_code": 200
}
```

### Error Responses

--------------------------------------------------------------------------------
