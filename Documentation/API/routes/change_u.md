# /a/change_u
Used to change the name of a user.

**URL** : `/a/change_u/`

**Method** : `POST`

**Auth required** : NO

**Header**

```json
{
    "room_id": UUIDv4,
    "user_id": UUIDv4,
    "new_user": "aph"
}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
    status: 200,
    message: "Success"
}
```

## Error Response

**Condition** : ?

**Code** : `500 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    status: 500,
    message: "Unknown Error",
    errID: errID
}
```

<br>

**Condition** : Client send a Request with missing Headers.

**Code** : `400 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    status: 400,
    message: "Missing Header"
}
```

<br>

**Condition** : Client send a Request with room_id that doesn't exist.

**Code** : `400 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    status: 400,
    message: "Room Does Not Exist"
}
```

<br>

**Condition** : Client send a Request with user_id that isn't assigned to the room with that particular room_id.

**Code** : `400 INTENRAL SERVER ERROR`

**Content** : 

```json
{
    status: 400,
    message: "User Not In Room"
}
```