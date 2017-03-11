# Get a Speaker

This endpoint is to be used to get details about a speaker.

## Resource

```
GET /speaker/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------------
id            | int  | yes      | ID of the speaker

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl -X GET "http://api.monctonhomeshow.engageitapp.com/v1/speakers/1"
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
    "id": 1,
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
  }
}
```

### Error Responses

--------------------------------------------------------------------------------

**Status-Code:** `400 Title Required`

```json
{
    "": ""
}
```
