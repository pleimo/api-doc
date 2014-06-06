Class: user
===========

Method: details
-----------
Format: __JSON__, __XML__
HTTP Supported: __GET__

> Get basic information about an user.

Example URLs:
-------------

Params:
-------

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

Sample Response:
----------------

```json
{
    "status": {
        "version": "1.0",
        "code": 200,
        "message": "success"
    },
    "user": {
        "id": "f0c2b1ada2c988673eb887f23270b684e6310ce6",
        "name": "Leonardo",
        "lastname": "Moreira",
        "email": "msn@leonardomoreira.com.br",
        "facebook_id": "1636057229",
        "language": "pt-BR",
        "image": {
            "small": "http://pleimo-images.s3.amazonaws.com/user/50/f/a/9/f/a/fa9faf8f176f12f844af7f36adb4cfdb.jpg",
            "medium": "http://pleimo-images.s3.amazonaws.com/user/100/f/a/9/f/a/fa9faf8f176f12f844af7f36adb4cfdb.jpg",
            "large": "http://pleimo-images.s3.amazonaws.com/user/180/f/a/9/f/a/fa9faf8f176f12f844af7f36adb4cfdb.jpg"
        },
        "currency": {
            "code": "BRL",
            "symbol": "R$"
        },
        "artists": [
            {
                "name": "deadmau5"
            },
            {
                "name": "Henrique Portugal"
            },
            {
                ...
            },
       ]
    }
}
```
