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
      "id": 8,
      "company_id": 2,
      "first_name": "Jay",
      "last_name": "Rodrigues",
      "title": null,
      "bio": null,
      "about_me": null,
      "company_name": "Development Account",
      "twitter": null,
      "google": null,
      "facebook": null,
      "instagram": null,
      "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
      "phone": null,
      "url": null,
      "session_data": [
        {
          "title": "Test sessions 2",
          "abstract": "Little info about session",
          "location": "center hall",
          "session_date": "2017-03-09",
          "start_time": "00:00:00"
        },
        {
          "title": "Test sessions 2",
          "abstract": "Little info about session",
          "location": "center hall",
          "session_date": "2017-03-09",
          "start_time": "02:08:00"
        }
      ]
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
