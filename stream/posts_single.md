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
    "content": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
    "picture": "",
    "post_by": 8,
    "date_time": 1489252612,
    "status": 1,
    "created_at": "2017-03-11 17:06:57",
    "updated_at": null,
    "button_text": "Check this out",
    "button_url": null,
    "image_url": null,
    "company_id": null,
    "is_moderated": 0,
    "post_type": 1,
    "avatar_file": "",
    "first_name": null,
    "last_name": null,
    "company_name": null,
    "like": [],
    "comment": [],
    "is_like": 0,
    "total_like": 0,
    "total_comment": 0
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
