# Auth endpoints

## Index

* [Sign in](#Sign-in)
* [Sign out](#Sign-out)

---

## Sign in
Sign in an account of provided email and password.

### Endpoint
POST `/auth/sign_in`

### Body

- `email`: **[String]** User email.
- `password`: **[String]**  User password.

### Success response

- **Status:** OK (200)
+ **Header:**
    - `access-token`: **[String]** Session access token.
    - `client`: **[String]** Session client.
    - `uid`: **[String]** Session UID (email). 
- **Body:**
```json
{
    "data": {
        "id": 1,
        "email": "email@example.com",
        "provider": "email",
        "uid": "email@example.com",
        "allow_password_change": false,
        "name": null,
        "nickname": null,
        "image": null
    }
}
```


---

## Sign out
Sign out an account of provided token.

### Endpoint
DELETE `/auth/sign_out`

### Header
- `access-token`: **[String]** Session access token.
- `client`: **[String]** Session client.
- `uid`: **[String]** Session UID (email). 

### Success response

- **Status:** OK (200)
- **Body:**
```json
{
    "success": true
}
```