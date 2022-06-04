# /a/create_r
Used to create a room.

**URL** : `/a/create_r/`

**Method** : `POST`

**Auth required** : NO

**Header**

```json
{}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
    "status": 200,
    "message": "Success"
}
```

## Error Response

**Condition** : ?

**Code** : `500 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    "status": 500,
    "message": "Unknown Error",
    "errID": errID
}
```