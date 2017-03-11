# update a comment for a post

This endpoint is to be used to update a comment for a post.

## Resource

```
PUT /posts/comment/{user_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | yes      | ID of the current user.


URL Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
post_id       | int    | yes      |
comment       | string | yes      |
status        | int    | no       | 0=inactive, 1=active. default 1

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
  "message": "Comment Updated successfully",
  "status_code": 200,
  "data": true
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
    "post_id": [
      "The post id field is required."
    ],
    "comment": [
      "The comment field is required."
    ]
  },
  "status_code": 422
}
```
