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
    "roomID": "9ca9e8cc-d8f6-4c6b-a097-025d380069a5",
    "users": [],
    "params": {
        "current_video": "",
        "time": 0
    }
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