# Add a like for a post

This endpoint is to be used to add a like for a post.

## Resource

```
POST /plus_like/{user_id}/{post_id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
user_id       | int  | yes      | ID of the current user.
post_id       | int  | yes      | Post ID.

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
```
