# TON Moji API
Public API of the TON Moji

## Authorization
You do not need to get a token to access our API. You can use it without authorization.

## Rate limit
10 requests per second

## Endpoint
``https://api.ton.ink/api/v1``

## Methods
### GET /getInfoByEmoji
Get user nickname by wallet address
#### Request
| Param   | Type   | Description                                                   |
|---------|--------|---------------------------------------------------------------|
| emoji* | String | Emoji you want to find |
#### Response
| Param   | Type   | Description                                                   |
|---------|--------|---------------------------------------------------------------|
| status | String - ok/error | Status of your request |
| message | String | Added to the response in case of an error. Error description. |
| data | Array | Emoji information |
| data.owner | String | Emoji owner's address  |
| data.name | String | Emoji owner's name  |
| data.description | String | Emoji owner's description  |
| data.links | Array | Links to social networks  |
| data.links[0].displayName | String | Name/domain  |
| data.links[0].url | String | Url |
