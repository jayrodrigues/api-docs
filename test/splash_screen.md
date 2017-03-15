### Splash Page

Update ads with image and image_url

https://github.com/jayrodrigues/api-docs/blob/master/ads/update.md

{{url}}/ads/3

```
curl -X POST -H "X-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjgsImlzcyI6Imh0dHBzOlwvXC9hcGkubW9uY3RvbmhvbWVzaG93LmVuZ2FnZWl0YXBwLmNvbVwvdjFcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg5NDYwOTgzLCJleHAiOjE0ODk4OTI5ODMsIm5iZiI6MTQ4OTQ2MDk4MywianRpIjoiOTk2MWI0NjFhZmQyNWMxNTk3NGFkOWUwNjUyNWRiZWEifQ.ptuZrvUK08JvotO_IAFiAZvBrQiF7EhDTGylYm0HR9Q" -H "Cache-Control: no-cache" -H "Postman-Token: f7d47850-59a7-d815-ce33-11bab3a81ba2" -H "Content-Type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW" -F "image=@if-logo-100px.png" -F "image_url=https://stg1.tieit.io/" "https://api.monctonhomeshow.engageitapp.com/v1/ads/3"
```

```json
{
  "message": "updated successfully",
  "status_code": 200,
  "data": null
}
```

get current active splash ads

https://github.com/jayrodrigues/api-docs/blob/master/ads/current.md

```
curl -X GET -H "x-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Cache-Control: no-cache" -H "Postman-Token: 579d7534-5753-bfbe-c25b-09feb35310a5" "https://api.monctonhomeshow.engageitapp.com/v1/ads/splash"
```

```json
{
  "message": "Current ads found",
  "status_code": 200,
  "data": {
    "id": 3,
    "name": "Splash ads",
    "image": "https://api.monctonhomeshow.engageitapp.com/uploads/banners/c6a80adc519d325a4796b0e5a691d6c7.png",
    "image_url": "https://stg1.tieit.io/",
    "is_current": 1,
    "user_id": 8,
    "button_text": "AWESOME",
    "button_url": null,
    "company_id": 1,
    "type": 3,
    "is_active": 1,
    "added_date": null,
    "schedule_date": "2017-03-12 23:00:00",
    "company_name": null,
    "company_city": null,
    "company_address": null
  }
}
```
