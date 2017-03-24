# Conference App API Documentation

## Introduction

This is the v1 version of the document.

### Base URL

```
http://api.monctonhomeshow.engageitapp.com/v1/
```

## Endpoints

### Sessions

- [**`GET`** /{lang}/sessions](/sessions/all.md)
- [**`GET`** /{lang}/sessions/{id}](sessions/single.md)
- [**`POST`** /sessions](sessions/create.md)
- [**`POST`** /sessions/{id}](sessions/update.md)

### Speakers

- [**`GET`** /speakers](/speakers/all.md)
- [**`GET`** /speakers/{id}](speakers/single.md)
- [**`POST`** /speakers](speakers/create.md)
- [**`POST`** /speakers/{id}](speakers/update.md)

### Notes

- [**`GET`** /notes](/notes/all.md)
- [**`GET`** /notes/{note_id}](notes/single.md)
- [**`GET`** /users/notes/{user_id}](notes/user_single.md)
- [**`POST`** /notes](notes/create.md)
- [**`POST`** /notes/{id}](notes/update.md)

### Users

- [**`POST`** /users/profile/{unique_device_id}](users/create_profile.md)
- [**`POST`** /users/{user_id}](users/update_profile.md)
- [**`GET`** /users/{user_id}](users/user_details.md)
- [**`GET`** /users/notes/{user_id}](notes/user_single.md)
- [**`GET`** /users/{unique_device_id}/{email}](users/user_details_by_param.md)

### Contacts

- [**`GET`** /contacts/{user_id}/{email}](contacts/get_contact_details.md)
- [**`POST`** /contacts/{id}](contacts/update.md)
- [**`GET`** /contacts/connect/{email}](contacts/link_contact.md)

### Attendees

- [**`GET`** /attendees/{user_id}](attendees/all.md)
- [**`GET`** /attendees/details/{email}](attendees/single.md)

### Authentication

- [**`POST`** /auth/login (for exhibitor login)](authentication/login.md)

### Device

- [**`POST`** /devices](authentication/add_this_device.md)

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

- [**`GET`** /posts](/stream/posts.md)
- [**`GET`** /posts/{user_id}](/stream/posts_user.md)
- [**`GET`** /admin/posts](/stream/admin_posts.md)
- [**`GET`** /admin/posts/{user_id}](/stream/admin_posts.md)
- [**`GET`** /posts/{user_id}/{post_id}](stream/posts_single.md)
- [**`POST`** /posts/{user_id}](stream/posts_create.md)
- [**`POST`** /posts/update/{post_id}](stream/posts_update.md)
- [**`POST`** /posts/comment/{user_id}](stream/post_comment.md)
- [**`PUT`** /posts/comment/{user_id}](stream/post_comment_update.md)
- [**`DELETE`** /posts/comment/{user_id}/{post_id}](stream/post_comment_delete.md)
- [**`POST`** /posts/rating/{user_id}/{post_id}/{rating}](stream/rating.md)

### Exhibitors

- [**`GET`** /{lang}/exhibitors](/exhibitors/all.md)
- [**`GET`** /{lang}/exhibitors/{id}](/exhibitors/single.md)
- [**`GET`** /exhibitors/verify/{email}](/exhibitors/retrieve_code.md)
- [**`GET`** /exhibitors/verify/{email}/{access_code}](/exhibitors/verify_code.md)
- [**`POST`** /exhibitors](exhibitors/create.md)
- [**`POST`** /exhibitors/{id}](exhibitors/update.md)

### Ads

- [**`GET`** /ads](/ads/all.md)
- [**`GET`** /ads/{ads_type}](/ads/current.md)
- [**`GET`** /ads/{ads_type}/{ads_id}](/ads/setCurrent.md)
- [**`POST`** /ads](/ads/create.md)
- [**`POST`** /ads/{ads_id}](/ads/update.md)
- [**`GET`** /ads/tracking/{ads_id}/{activity_type}](/ads/tracking.md)
- [**`GET`** /ads/tracking/{ads_id}/{activity_type}/{user_id}](/ads/tracking.md)
- [**`GET`** /ads_tracking_details/{ads_id}](/ads/tracking_details.md)

### Groups

- [**`GET`** /groups/{user_id}](groups/all.md)
- [**`GET`** /groups/{user_id}/{email}](groups/byemail.md)
- [**`POST`** /groups/add (Add contact to group)](groups/add_contact_to_group.md)
- [**`POST`** /groups/remove (Remove contact from group)](groups/remove_contact_from_group.md)
