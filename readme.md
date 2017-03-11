# Conference App API Documentation

## Introduction

This is the v1 version of the document.

### Base URL

```
http://api.monctonhomeshow.engageitapp.com/v1/
```

## Endpoints

### Sessions

- [**`GET`** /sessions](/sessions/all.md)
- [**`GET`** /sessions/{id}](sessions/single.md)
- [**`POST`** /sessions](sessions/create.md)
- [**`POST`** /sessions/{id}](sessions/update.md)

### Speakers

- [**`GET`** /speakers](/speakers/all.md)
- [**`GET`** /speakers/{id}](speakers/single.md)
- [**`POST`** /speakers](speakers/create.md)
- [**`POST`** /speakers/{id}](speakers/update.md)

### Users

- [**`POST`** /users/profile/{unique_device_id}](users/create_profile.md)
- [**`PUT`** /users/profile/{user_id}](users/update_profile.md)
- [**`GET`** /auth/users/{user_id}](users/user_details.md)

### Contacts

- [**`GET`** /contacts/{user_id}/{email}](contacts/get_contact_details.md)
- [**`POST`** /contacts/{id}](contacts/update.md)

### Authentication

- [**`POST`** /auth/login (for exhibitor login)](authentication/login.md)

### Device

- [**`POST`** /add_this_device](authentication/add_this_device.md)

### Tracks

- [**`GET`** /tracks](/tracks/all.md)
- [**`GET`** /tracks/{id}](tracks/single.md)
- [**`POST`** /tracks](tracks/create.md)
- [**`POST`** /tracks/{id}](tracks/update.md)

### Companies

- [**`GET`** /companies](/companies/all.md)
- [**`GET`** /companies/{id}](companies/single.md)
- [**`POST`** /companies](companies/create.md)
- [**`POST`** /companies/{id}](companies/update.md)

### Streaming

- [**`GET`** /posts/{user_id}](/stream/posts.md)
- [**`GET`** /posts/{user_id}/{post_id}](stream/posts_single.md)
- [**`POST`** /posts/{user_id}](stream/posts_create.md)
- [**`PUT`** /posts/{post_id}](stream/posts_update.md)
- [**`POST`** /posts/comment/{user_id}](stream/post_comment.md)
- [**`PUT`** /posts/comment/{user_id}](stream/post_comment_update.md)
- [**`DELETE`** /posts/comment/{user_id}/{post_id}](stream/post_comment_delete.md)
- [**`POST`** /posts/rating/{user_id}/{post_id}/{rating}](stream/rating.md)

### Exhibitors

- [**`GET`** /exhibitors](/exhibitors/all.md)
- [**`GET`** /exhibitors/{id}](/exhibitors/single.md)
- [**`GET`** /exhibitors/retrieve_code/{email}](/exhibitors/retrieve_code.md)
- [**`POST`** /exhibitors](exhibitors/create.md)
- [**`POST`** /exhibitors/{id}](exhibitors/update.md)
