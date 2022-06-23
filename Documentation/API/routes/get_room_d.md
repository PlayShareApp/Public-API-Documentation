# /a/get_room_d
Used to create a room.

**URL** : `/a/get_room_d/`

**Method** : `POST`

**Auth required** : NO

**Header**

```json
{
    "room_id": UUIDv4,
}
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
        "time": 0,
        "state:" false
    }
}
```

## Error Response

**Condition** : Client send a Request with missing Headers.

**Code** : `400 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    "status": 400,
    "message": "Missing Header"
}
```

<br>

**Condition** : Client send a Request with room_id that doesn't exist.

**Code** : `400 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    "status": 400,
    "message": "Room Does Not Exist"
}
```

<br>

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