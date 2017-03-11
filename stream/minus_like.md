# Minus a like for a post

This endpoint is to be used to minus like from a post.

## Resource

```
POST /minus_like/{user_id}/{post_id}
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
  "message": "Post not found to unlike",
  "status_code": 400
}
```
