</> Markdown 

# JSONPlaceholder API Documentation (Sample)

This sample documentation project uses the JSONPlaceholder API to demonstrate basic API functionality.

---

## GET /posts/{id}

Retrieves a single post by its unique ID.

---

### When to use this endpoint

This endpoint retrieves the details of a specific post. It can be used to display content in an application or to review a single record.

---

### Example Request

```bash
curl https://jsonplaceholder.typicode.com/posts/1
```

### Example Response
```json
{
        "userId": 1,
        "id": 1,
        "title": "Sample title",
        "body": "Sample body"
}
```

### Notes

- The `id` must be a positive integer.
- If the post does not exist, the API returns an empty object.
---

## GET /posts

Returns a list of posts.

---

### When to use this endpoint

This endpoint shows multiple posts in the database.

---

### Example Request

```bash
curl https://jsonplaceholder.typicode.com/posts
```
---

### Example Response

```json
 [
    {
        "userId": 1,
        "id": 1,
        "title": "Sample title",
        "body": "Sample body"
    }
    
  ]
```

### Notes

- This endpoint will return a list of posts.