# delete a comment for a post

This endpoint is to be used to delete a comment for a post. To inactive a comment use /post_comment_update/{user_id} endpoint

## Resource

```
POST /posts/comment/delete/{user_id}/{post_id}
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
Created successfully

**Status-Code:** `200 OK`

```json
{
  "message": "Comment deleted successfully",
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
  "message": "Can't delete the record",
  "status_code": 400
}
```
