# List all Posts

This endpoint is to be retrieve a post details with total like comment count.

## Resource

```
GET /posts/{user_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
post_id       | int  | yes      | ID of the post.

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/posts/1'
```

### Response

--------------------------------------------------------------------------------
Record found

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
      "post_by": 8,
      "date_time": 1489264319,
      "status": 1,
      "created_at": "2017-03-11 17:06:57",
      "updated_at": null,
      "button_text": "Check this out",
      "button_url": null,
      "image_url": null,
      "company_id": null,
      "is_moderated": 1,
      "post_type": 1,
      "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg",
      "first_name": "Jay",
      "last_name": "Rodrigues",
      "company_name": "Development Account",
      "sponsor_post_company_name": null,
      "sponsor_company_logo": null,
      "total_like": 1,
      "total_comment": 2,
      "is_like": 1
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
