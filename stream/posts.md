# List all Posts

This endpoint is to be retrieve a post details with total like comment count.

## Resource

```
GET /posts
```

## Parameters

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/posts'
```

### Response

--------------------------------------------------------------------------------
If post_type = 1 (Normal)

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
      "id": 1,
      "content": "new update",
      "picture": "",
      "posted_at": 1489264319,
      "status": 1,
      "created_at": "2017-03-11 17:06:57",
      "updated_at": null,
      "is_moderated": 1,
      "post_type": 1,
      "posted_by": {
        "user_id": 8,
        "first_name": "Jay",
        "last_name": "Rodrigues",
        "company_name": "Development Account",
        "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg"
      },
      "total_like": 1,
      "total_comment": 2
    }
  ]
}
```

If post_type = 2 (Sponsor)

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": [
    {
      "id": 1,
      "content": "new update",
      "picture": "",
      "posted_at": 1489264319,
      "status": 1,
      "created_at": "2017-03-11 17:06:57",
      "updated_at": null,
      "is_moderated": 1,
      "post_type": 2,
      "sponsor_company_logo": null,
      "posted_by": {
        "user_id": 8,
        "first_name": "Jay",
        "last_name": "Rodrigues",
        "company_name": "Development Account",
        "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg"
      },
      "sponsor_ad": {
        "sponsor_post_company_name": null,
        "button_text": "Check this out",
        "button_url": null,
        "image_url": null
      },
      "total_like": 1,
      "total_comment": 2
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

**Status-Code:** ``

`json`
