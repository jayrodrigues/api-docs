# List single Post

This endpoint is to be retrieve details of a post with total like comment count. Also this endpoint will return is current user like post already or not.

## Resource

```
GET /posts/{user_id}/{post_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | yes      | ID of the current user.
post_id       | int  | yes      | ID of the post.

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/posts/8/1'
```

### Response

--------------------------------------------------------------------------------
Record found

**Status-Code:** `200 OK`

```json
{
  "message": "Data found",
  "status_code": 200,
  "data": {
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
    "company_name": null,
    "like": [
      {
        "id": 3,
        "post_id": 1,
        "user_id": 8,
        "date_time": "0000-00-00 00:00:00",
        "status": 1,
        "created_at": null,
        "updated_at": null,
        "first_name": "Jay",
        "last_name": "Rodrigues",
        "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg"
      }
    ],
    "comment": [
      {
        "id": 4,
        "post_id": 1,
        "user_id": 8,
        "comment": "This is first comment",
        "date_time": "0000-00-00 00:00:00",
        "status": 1,
        "created_at": "2017-03-12 13:08:35",
        "updated_at": "2017-03-12 13:08:35",
        "first_name": "Jay",
        "last_name": "Rodrigues",
        "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg"
      },
      {
        "id": 3,
        "post_id": 1,
        "user_id": 8,
        "comment": "new update",
        "date_time": "0000-00-00 00:00:00",
        "status": 1,
        "created_at": "2017-03-11 20:24:51",
        "updated_at": "2017-03-11 20:29:25",
        "first_name": "Jay",
        "last_name": "Rodrigues",
        "avatar_file": "http://awesome.dev/engageitapimoncton/public/uploads/profile_pics/52e601c07640ffae2626e516a0489b00.jpg"
      }
    ],
    "is_like": 1,
    "total_like": 1,
    "total_comment": 2
  }
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
