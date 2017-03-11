# Update post

This endpoint is to be used to update a post.

## Resource

```
POST /post_update/{post_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
post_id       | int  | yes      | ID of the post.


POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
content       | string | yes      |
picture       | file   | no       |
is_moderated  | int    | no       | default 0. set 1 to publish at once
status        | int    | no       | default 1. 0=false, 1=true
button_text   | string | no       |
button_url    | string | no       |
image_url     | string | no       |
company_id    | int    | no       |
post_type     | int    | no       | 1-normal, 2=sponsor. default 1

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl ''
```

### Response

--------------------------------------------------------------------------------
Created successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Post updated",
  "status_code": 200,
  "data": 1
}
```

### Error Responses

--------------------------------------------------------------------------------
Validation Error

**Status-Code:** `422 Unprocessable Entity`

```json
{
  "message": "Can't create new record",
  "errors": {
    "content": [
      "The content field is required."
    ]
  },
  "status_code": 422
}
```

can't upload picture

**Status-Code:** `500 Internal Server Error`

```json
{
  "message": "The target directory `uploads/posts` does not exists or is not writable",
  "status_code": 500
}
```

Unsupported Media Type

**Status-Code:** `415 Unsupported Media Type`

```json
{
  "message": "Please upload a valid file (png/jpeg/gif)",
  "status_code": 415
}
```
