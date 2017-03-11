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

- [**`POST`** /user/create_profile](users/create_profile.md)
- [**`POST`** /user/update_profile/{user_id}](users/update_profile.md)
- [**`GET`** /auth/user/{user_id}](users/user_details.md)

### Contacts

- [**`POST`** /get_contact_details/{user_id}](contacts/get_contact_details.md)
- [**`POST`** /contacts/{id}](contacts/update.md)

### Authentication

- [**`POST`** /auth/login (for exhibitor login)](authentication/login.md)

### Tracks

- [**`GET`** /tracks](/tracks/all.md)
- [**`GET`** /tracks/{id}](tracks/single.md)
- [**`POST`** /tracks](tracks/create.md)
- [**`POST`** /tracks/{id}](tracks/update.md)

### Streaming

- [**`GET`** /posts/{user_id}](/stream/posts.md)
- [**`GET`** /post_details/{user_id}/{post_id}](stream/posts_single.md)
- [**`POST`** /posts/{user_id}](stream/posts_create.md)
- [**`PUT`** /posts/{post_id}](stream/posts_update.md)
- [**`POST`** /posts/comment/{user_id}](stream/post_comment.md)
- [**`PUT`** /posts/comment/{user_id}](stream/post_comment_update.md)
- [**`DELETE`** /posts/comment/{user_id}/{post_id}](stream/post_comment_delete.md)
- [**`POST`** /posts/rating/{user_id}/{post_id}/{rating}](stream/rating.md)
