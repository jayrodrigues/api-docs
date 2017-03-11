# Update User Contact Information

This endpoint is to be used to update a user contact information.

## Resource

```
POST /contacts/{id}
```

## Parameters

URI Parameter | Type | Required | Description
:------------ | :--- | :------- | :----------
id            | int  | yes      | ID of the user_contact

POST Parameter | Type   | Required | Description
:------------ | :----- | :------- | :----------
first_name    | string | no       |
last_name     | string | no       |
company       | int    | no       | company id
city          | string | no       |
state         | string | no       |
country       | string | no       |
phone         | string | no       |
avatar_file   | file   | no       | profile picture
zip           | string | no       |
address       | string | no       |
linkedin      | string | no       |
twitter       | string | no       |
url           | string | no       |
company_email | string | no       |
facebook      | string | no       |
instagram     | string | no       |
pinterest     | string | no       |
youtube       | string | no       |
google        | string | no       |
about_me      | text   | no       |
bio           | text   | no       |
position      | string | no       |

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
  "message": "Your changes have been updated successfully",
  "status_code": 200
}
```

### Error Responses

--------------------------------------------------------------------------------
