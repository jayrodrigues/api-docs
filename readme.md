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

### Tracks

- [**`GET`** /tracks](/tracks/all.md)
- [**`GET`** /tracks/{id}](tracks/single.md)
- [**`POST`** /tracks](tracks/create.md)
- [**`POST`** /tracks/{id}](tracks/update.md)

### Streaming

- [**`GET`** /posts/{user_id}](/stream/posts.md)
- [**`GET`** /post_details/{post_id}](stream/posts_single.md)
- [**`POST`** /posts/{user_id}](stream/posts_create.md)
- [**`POST`** /post_update/{post_id}](stream/posts_update.md)
- [**`POST`** /posts_comment/{user_id}](stream/posts_comment.md)
- [**`POST`** /post_comment_update/{post_id}](stream/posts_comment_update.md)
- [**`POST`** /tracks/{id}](tracks/update.md)
