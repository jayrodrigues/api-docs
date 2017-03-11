# List all Tracks

This endpoint is to be retrieve a post details with total like comment count.

## Resource

```
GET /post_details/{post_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
post_id       | int  | yes      | ID of the post.

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl 'http://api.monctonhomeshow.engageitapp.com/v1/post_details/1'
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
    "date_time": 0,
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