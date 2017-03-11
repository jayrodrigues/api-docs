# Create New comment for a post

This endpoint is to be used to create new comment for a post.

## Resource

```
POST /post_comment/{user_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | yes      | ID of the current user.


POST Parameter | Type   | Required | Description
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
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "post_id": "1",
    "comment": "Hello ",
    "date_time": 1489255103,
    "user_id": "8",
    "status": 1,
    "updated_at": "2017-03-11 17:58:23",
    "created_at": "2017-03-11 17:58:23",
    "id": 1
  }
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
