# Add this device

This endpoint is to be used to add new device and get unique device id. and this unique device id need to send on profile creation or login

## Resource

```
POST /add_this_device
```

## Parameters

URI Parameter     | Type   | Required | Description
:---------------- | :----- | :------- | :----------------------------
device_identifier | string | yes       |
device_type       | int    | yes       | 0 = iOS; 1 = Android (verify)
device_os         | string | no        |
device_model      | string | no        |

## Example

### Request

--------------------------------------------------------------------------------

```
curl -X POST -H ""
```

### Response

--------------------------------------------------------------------------------

**Status-Code:** `200 OK`

```json
{
  "message": "Device added successfully",
  "status_code": 200,
  "unique_device_id": "f1af518194ed957"
}
```

### Error Responses

--------------------------------------------------------------------------------
if device already added
**Status-Code:** `200`

```json
{
  "message": "Device already added",
  "status_code": 200,
  "unique_device_id": "f1af518194ed957"
}
```
