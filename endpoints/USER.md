Class: user
===========

Method: details
-----------
Format: __JSON__, __XML__ <br>
HTTP Supported: __GET__

> Get basic information about an user.

#### Example URLs:
__JSON:__ `http://api.pleimo.com/user/details/json?id=f0c2b1ada2c988673eb887f23270b684e6310ce6&api_key=bd7203c61a13f6a8a6a039255cd26359` <br>
__XML:__ `http://api.pleimo.com/user/details/xml?id=f0c2b1ada2c988673eb887f23270b684e6310ce6&api_key=bd7203c61a13f6a8a6a039255cd26359`

#### Params:
| Parameter     | Required?     | Value      | Description          |
| ------------- | ------------- | ---------- | -------------------- |
| id            | yes           | `string`   | The User token (ID)  |

#### Sample Response:
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

#### Version:
__v1.0__ <br>
*Last Revision: 2013/11/22*