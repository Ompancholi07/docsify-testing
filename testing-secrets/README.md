  <!-- <h1 align="center">Videomagic Backend APIs</h1>

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


 -->
 # Release Structure and Versioning

## Overview

This document provides an outline of our release structure and versioning strategy for production releases. Proper versioning and release management are essential to maintaining a structured and organized software development process.

## Table of Contents

- [Versioning Scheme](#versioning-scheme)
- [Release Types](#release-types)
- [Release Workflow](#release-workflow)
- [Version History](#version-history)

## Versioning Scheme

We follow the Semantic Versioning (SemVer) scheme for version numbers. A version number consists of three segments: `MAJOR.MINOR.PATCH`. Each segment has a specific meaning:
- `MAJOR`: Incremented for significant and potentially backward-incompatible changes.
- `MINOR`: Incremented for backward-compatible new features and enhancements.
- `PATCH`: Incremented for backward-compatible bug fixes and minor improvements.

Example: `1.2.3`

## Release Types

We use the following release types to categorize our releases:

1. **Major Release (X.0.0):** Significant and potentially breaking changes, major new features.
2. **Minor Release (X.Y.0):** New features and enhancements that are backward-compatible.
3. **Patch Release (X.Y.Z):** Bug fixes, minor improvements, and backward-compatible changes.

## Release Workflow

Our release workflow includes the following stages:

1. **Development:** All changes and new features are developed on feature branches.
2. **Testing:** Comprehensive testing, including unit tests, integration tests, and user acceptance testing, is performed on the feature branch.
3. **Code Review:** A peer code review is conducted to ensure code quality and adherence to coding standards.
4. **Merging:** Approved changes are merged into the main development branch.
5. **Version Bumping:** Update the version number in the project configuration files.
6. **Build and Packaging:** Generate deployable artifacts.
7. **Deployment:** Deploy to staging or pre-production environments for further testing.
8. **Quality Assurance:** Comprehensive testing in the staging environment.
9. **Release Candidate:** Prepare the release candidate for production.
10. **Release:** Deploy the release candidate to the production environment.
11. **Post-release:** Monitor production, address issues, and plan for the next release.

## Version History

| Version | Release Date | Description |
| ------- | ------------ | ----------- |
| 1.0.0   | YYYY-MM-DD   | - Initial release |
| 1.1.0   | YYYY-MM-DD   | - Added feature X<br>- Fixed issue Y |
| 1.1.1   | YYYY-MM-DD   | - Fixed critical bug Z |
| 2.0.0   | YYYY-MM-DD   | - Major redesign<br>- New API endpoints |

Please note that this document provides a high-level overview of our release structure and versioning. Detailed release notes and documentation should accompany each release to provide additional context and information.


