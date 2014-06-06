Pleimo API
==========

API integration for Pleimo Services.

Where do I start?
=================

You must have your own API key to make use of the Pleimo API. To obtain a key, contact developer@pleimo.com.

Overview
========

The Pleimo API allows you to call methods that respond in JSON or XML. You can call a method by using an GET, POST, PUT or DELETE.

To retrieve, use:
`http://api.pleimo.com/v1/[class]/[method].[format]?[parameters] along with method specific arguments.`

Example:
`http://api.pleimo.com/artist/search/xml?name=medulla&api_key=bd7203c61a13f6a8a6a039255cd26359`

Request HTTP Methods: GET, POST, PUT, DELETE
Response Formats: JSON, XML

Check supported HTTP method in individual class documentation.
This API does not support SSL in this version.

Rate Limits
===========

No rate limits for now ;)


Endpoints
=========


Authentication
==============

Logging your users into our products is supported through OAuth 2. Several apps support login via API tokens.

```json
[
  {
    "id": 605816632,
    "name": "BCX",
    "description": "The Next Generation",
    "updated_at": "2012-03-23T13:55:43-05:00",
    "url": "https://basecamp.com/999999999/api/v1/projects/605816632-bcx.json",
    "archived": false,
    "starred": true
  },
  {
    "id": 684146117,
    "name": "Nothing here!",
    "description": null,
    "updated_at": "2012-03-22T16:56:51-05:00",
    "url": "https://basecamp.com/999999999/api/v1/projects/684146117-nothing-here.json",
    "archived": false,
    "starred": false
  }
]
```

Errors
======

All known errors cause the resource to return HTTP error code header together with a JSON array containing at least 'status' and 'error' keys describing the source of error.

* `403` Forbidden : Invalid authorization credentials.
* `404` Not Found : Unsupported method, format or required arguments.
* `422` Unprocessable Entity : One or more of the required fields didn't include valid data.

Help us make it better
======================

Please tell us how we can make the APIs better. If you have a specific feature request or if you found a bug, please contact developer@pleimo.com