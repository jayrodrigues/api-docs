# Like unlike any post

This endpoint is to be used to like/unlike any post.

## Resource

```
POST /posts/rating/{user_id}/{post_id}/{rating}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | yes      | ID of the current user.
post_id       | int  | yes      | Post ID.
rating        | string  | yes   | like or unlike

## Example

### Request

--------------------------------------------------------------------------------

```curl
curl ''
```

### Response

--------------------------------------------------------------------------------
like added successfully

**Status-Code:** `200 OK`

```json
{
  "message": "You liked the post",
  "status_code": 200,
  "data": {
    "status": 1,
    "post_id": "1",
    "user_id": "8",
    "date_time": 1489255778,
    "id": 1
  }
}

{
  "message": "You unliked the post",
  "status_code": 200,
  "data": true
}


```

### Error Responses

--------------------------------------------------------------------------------
Validation Error

**Status-Code:** `400`

```json
{
  "message": "Post not found to like",
  "status_code": 400
}

{
  "message": "No like found to unlike",
  "status_code": 200,
}

{
  "message": "You already like the post",
  "status_code": 200,
}
```
