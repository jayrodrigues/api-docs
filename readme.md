# Conference App API Documentation

## Introduction

This is the v1 version of the document.

### Base URL

```
https://api.engageitapp.com/v1/monctonhomeshow2017/
```

## Endpoints

### Registration and Authentication

- [**`GET`** /auth/login](/authentication/login.md)
- [**`GET`** /auth/users](/authentication/users.md)

### Authentication

- [**`GET`** /users/login](/users/login.md)
- [**`GET`** /users/social_login](/users/social_login.md) **
- [**`GET`** /users/forgot_password](/users/forgot_password.md)

### Profile

- [**`GET`** /users/profile](/users/profile.md)
- [**`GET`** /users/lic_verify](/users/lic_verify.md)
- [**`GET`** /users/user (data)](/users/user_data.md)
- [**`GET`** /users/user (image)]

### Companies

- [**`GET`** /search/list]
- [**`GET`** /ride/ride_detail]
- [**`GET`** /ride/book_ride]

### Sponsors

- [**`POST`** /ride/offer_ride](/rides/one-off/step1.md)
- [**`POST`** /ride/update_price](rides/update_price.md)
- [**`GET`** /ride/offer_ride]
- [**`POST`** /ride/update_price]
- [**`POST`** /ride/update_price]

### Exhibitors

- [**`POST`** /ride/offer_ride](/rides/regular/step1.md)
- [**`POST`** /ride/update_price]
- [**`GET`** /ride/offer_ride] -

### Sessions

- [**`GET`** /sessions](/sessions/list_sessions.md)
- [**`GET`** /sessions/{id}](/sessions/get_sessions.md)
- [**`POST`** /sessions/](/sessions/create_session.md)
- [**`POST`** /sessions/{id}](/sessions/update_session.md)

### Tracks

- [**`GET`** /my_trips/handle_action](/requests/my_trips/passenger.md)
- [**`GET`** /my_trips/handle_action](/requests/my_trips/passenger_past.md)
- [**`POST`** /my_trips/handle_action] (cancel passenger)

### Speakers

- **[`GET /settings`](/users/com)**
- [**`GET`** /settings/change_password](/settings/change_password.md)
- [**`GET`** /settings/personal_info](/settings/personal_info.md)
- [**`GET`** /settings/authentication]
- [**`GET`** /settings/preference](/settings/preference.md)

### Notes

- [**`GET`** /settings/load_makes](/settings/load_makes.md)
- [**`GET`** /settings/load_models](/settings/load_models.md)
- [**`GET`** /settings/co2_emission](/settings/co2_emission.md)
- [**`GET`** /settings/veh_delete](/settings/veh_delete.md)
- [**`GET`** /settings/vehicle](/settings/vehicle.md)
- [**`GET`** /settings/manage_veh](/settings/manage_veh.md)

### Groups

- [**`GET`** /message]
- [**`GET`** /message/unread](/message/unread.md)
- [**`GET`** /message/inbox](/message/inbox.md)
- [**`GET`** /message/detail](/message/detail.md)
- [**`POST`** /message/send_batch_message](/message/send_batch_message.md)

### Ads

- [**`GET`** /ratings]
- [**`POST`** /ratings/rating_pending](/ratings/rating_pending.md)
- [**`POST`** /ratings/rating_received](/ratings/rating_received.md)
- [**`POST`** /ratings/rating_given](/ratings/rating_given.md)
- [**`POST`** /ratings/ratings/rating_campanign](/ratings/rating_campanign.md)
- [**`POST`** /ratings/ratings/rating_campanign](/ratings/rating_campanign_after.md)
