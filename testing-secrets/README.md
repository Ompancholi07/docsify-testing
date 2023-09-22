  <h1 align="center">Videomagic Backend APIs</h1>

# API Documentation

Welcome to the documentation for our API. This document provides detailed information about the endpoints, request methods, parameters, and response formats for our API.

## Table of Contents

- [Introduction](#introduction)
- [Authentication](#authentication)
- [API Endpoints](#endpoints)
  - [synthesia-automation](#endpoint-1)
  - [disable-menu](#endpoint-2)
- [Conclusion](#conclusion)

## Introduction

**1. _synthesia-automation API_** helps the user create customised AI generated videos with custom message. The user has freedom to adjust the Avatar, voice and has 100+ language options.

**2. _disable-menu API_** is an admin feature created for the admin to control the main-menu and sub-menus of the admin panel's menu page. The API helps to enable or disable the menu from admin panel as well as the UI.

## Authentication

Explain how users can authenticate with your API, whether it uses API keys, OAuth, or another method.

## API Endpoints

Here we are working on demo documentation of synthesia API and disable-menu API

### [synthesia-automation](#endpoint-1)

#### `POST /https://api.synthesia.io/v2/videos`

This API is used for video creation using synthesia feature.

##### Request

- **URL:** `/https://api.synthesia.io/v2/videos`
- **Method:** `POST`
- **Parameters:**
  - Parameter 1: 
```
{
    "test": true,
    "input": [{
        "scriptText": "Hi, this is demo from OM",
        "avatar": "laura_costume1_cameraA",
        "background": "warm_white"
    }],
     "soundtrack": "urban"
}
```

##### Response

- **Status Code:** 200 OK
- **Response Body:** 
```
{
    "createdAt": 1695288113,
    "id": "2cc145e4-dc88-4859-9726-039e9e428326",
    "lastUpdatedAt": 1695288113,
    "status": "in_progress",
    "visibility": "private"
}
```

### [disable-menu API](#endpoint-2)

#### `PUT /https://dev-api.videomagic.app/disable-menu/`

Description of what this endpoint does.

##### Request

- **URL:** `/https://dev-api.videomagic.app/disable-menu/`
- **Method:** `PUT`
- **Parameters:** 
  - Parameter 1: 
```
{
    "id": "4e4cb2f5-90ee-4565-9d71-64ec4bae2d4e",
    "value": 1
}
```

##### Response

- **Status Code:** 201 Created
- **Response Body:** 
```
{
        status: "success",
        message: "Record updated successfully",
        data: Record with id :4e4cb2f5-90ee-4565-9d71-64ec4bae2d4e is updated
      };
```


## Conclusion

This is just a sample documentation for our backend APIS. In the same way we can created an entire documentation for all the APIs. Please verify and suggest your views [here](https://github.com/orgs/videomagicllc/projects/20/views/1?filterQuery=om&pane=issue&itemId=39328461).

---



