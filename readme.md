</> Markdown 

# JSONPlaceholder API Documentation (Sample)

This repository contains a sample API documentation project created with Markdown and GitHub to demonstrate technical writing skills.

---
## Overview

This documentation demonstrates basic API concets using the JSONPlaceholder API, including how to make requests and interpret responses.

---
## Getting Started

JSONPlaceholder is a REST API that provides sample data for testing and learning. It allows you to retrieve information about resources such as posts, users, and comments by sending HTTP requests to specific endpoints.

**Base URL:** https://jsonplaceholder.typicode.com

```bash
curl https://jsonplaceholder.typicode.com/posts/1 
```

```json
{
  "userId": 1,
  "id": 1,
  "title": "...",
  "body": "..."
}
```

The response returns a single post object. The `id` uniquely identifies the post, while `userId` indicates the user who created it. The `title` provides a short summary of the post, and the `body` contains the full content. Together, these four fields describe the key attributes of a post and can be used to display or organize data in an application.

You have successfully made your first request and retrieved a post from the API.

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

This endpoint retrieves a collection of posts.

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