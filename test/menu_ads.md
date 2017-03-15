### Menu Ads

Update ads with button_text and button_url

https://github.com/jayrodrigues/api-docs/blob/master/ads/update.md

{{url}}/ads/4

```
curl -X POST -H "X-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjgsImlzcyI6Imh0dHBzOlwvXC9hcGkubW9uY3RvbmhvbWVzaG93LmVuZ2FnZWl0YXBwLmNvbVwvdjFcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg5NDYwOTgzLCJleHAiOjE0ODk4OTI5ODMsIm5iZiI6MTQ4OTQ2MDk4MywianRpIjoiOTk2MWI0NjFhZmQyNWMxNTk3NGFkOWUwNjUyNWRiZWEifQ.ptuZrvUK08JvotO_IAFiAZvBrQiF7EhDTGylYm0HR9Q" -H "Cache-Control: no-cache" -H "Postman-Token: f16b236b-a8e7-b1ef-c378-cd6a66761822" -H "Content-Type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW" -F "button_url=https://stg1.tieit.io/" -F "button_text=Ads Menu" "https://api.monctonhomeshow.engageitapp.com/v1/ads/4"
```

```json
{
  "message": "updated successfully",
  "status_code": 200,
  "data": null
}
```

set 4 id ads as current active menu ads

https://github.com/jayrodrigues/api-docs/blob/master/ads/setCurrent.md


```
curl -X GET -H "x-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjgsImlzcyI6Imh0dHBzOlwvXC9hcGkubW9uY3RvbmhvbWVzaG93LmVuZ2FnZWl0YXBwLmNvbVwvdjFcL2F1dGhcL2xvZ2luIiwiaWF0IjoxNDg5NTQ1MDQ2LCJleHAiOjE0ODk5NzcwNDYsIm5iZiI6MTQ4OTU0NTA0NiwianRpIjoiOWVlMjZmOWUxMzYxYjYzZDRhMGYxNTA4OTAzNzZkYjgifQ._So930-kuWTCWW44UjTJ4h--brvIYwy2842ceR8b2lA" -H "Cache-Control: no-cache" -H "Postman-Token: 28daeac3-0613-6ddc-8ad5-3d8642627c2a" "https://api.monctonhomeshow.engageitapp.com/v1/ads/menu/4"
```

```json
{
  "message": "Activated as current ads successfully",
  "status_code": 200,
  "data": {
    "id": 4,
    "name": "Menu Ads update",
    "image": null,
    "image_url": null,
    "is_current": 1,
    "user_id": 8,
    "button_text": "Ads Menu",
    "button_url": "https://stg1.tieit.io/",
    "company_id": 1,
    "type": 1,
    "is_active": 1,
    "added_date": null,
    "schedule_date": "2017-03-12 23:00:00"
  }
}
```

get current active menu ads {{url}}/ads/menu

https://github.com/jayrodrigues/api-docs/blob/master/ads/current.md

```
curl -X GET -H "x-key: 5ycd5F45WjkwpL6A@HGqSU242jbjOYQGD7D@qvXQU*uk@vWW8*e$p5p6Wd4krT*1" -H "Cache-Control: no-cache" -H "Postman-Token: 7c2a0dd7-b557-d00d-941b-398c3fb638b0" "https://api.monctonhomeshow.engageitapp.com/v1/ads/menu"
```

```json
{
  "message": "Current ads found",
  "status_code": 200,
  "data": {
    "id": 4,
    "name": "Menu Ads update",
    "image": null,
    "image_url": null,
    "is_current": 1,
    "user_id": 8,
    "button_text": "Ads Menu",
    "button_url": "https://stg1.tieit.io/",
    "company_id": 1,
    "type": 1,
    "is_active": 1,
    "added_date": null,
    "schedule_date": "2017-03-12 23:00:00",
    "company_name": null,
    "company_city": null,
    "company_address": null
  }
}
```
