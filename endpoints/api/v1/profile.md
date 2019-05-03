# Profile endpoints

## Index

* [Read single](#Read-single)

---

## Read single
Return a profile by id.

### Endpoint
GET `/api/v1/profiles/:id`

### Header
- `access-token`: **[String]** Session access token.
- `client`: **[String]** Session client.
- `uid`: **[String]** Session UID (email). 

### Success response

- **Status:** OK (200)
- **Body:**
```json
{
    "id": 1,
    "first_name": "Lorem",
    "last_name": "Ipsum",
    "created_at": "2019-05-03T18:01:57.836Z",
    "updated_at": "2019-05-03T18:01:57.836Z",
    "full_name": "Lorem Ipsum"
}
```