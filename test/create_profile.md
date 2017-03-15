### Create a dummy profile

To create a profile first you will need unique_device_id. so, lets create new device and generate unique_device_id

https://github.com/jayrodrigues/api-docs/blob/master/authentication/add_this_device.md

```
curl -X POST -H "X-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Cache-Control: no-cache" -H "Postman-Token: 42fc1ae4-66fe-3fb4-42fa-85813df4de98" -H "Content-Type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW" -F "device_identifier=lksjdklf564s6d7f68sre" -F "device_type=1" "https://api.monctonhomeshow.engageitapp.com/v1/devices"
```

```json
{
  "message": "Device added successfully",
  "status_code": 200,
  "unique_device_id": "b1e0f66ca9a366a"
}
```

now with this unique_device_id lets create a profile

https://github.com/jayrodrigues/api-docs/blob/master/users/create_profile.md


```
curl -X POST -H "X-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Cache-Control: no-cache" -H "Postman-Token: b32067a3-76ec-49d4-20d5-9f432fc03bc4" -H "Content-Type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW" -F "email=hasanmehdi89@gmail.com" "https://api.monctonhomeshow.engageitapp.com/v1/users/profile/b1e0f66ca9a366a"
```

```json
{
  "message": "Created successfully",
  "status_code": 200,
  "data": {
    "email": "hasanmehdi89+3@gmail.com",
    "id": 12
  }
}
```
