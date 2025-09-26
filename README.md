# Typicode Test API

This project provides a Postman collection for interacting with a typical blog post and comments API. The collection covers all standard CRUD operations for blog posts and allows you to retrieve comments, with support for filtering and pagination.

## Overview

The Typicode Test API collection is designed to help developers and testers quickly interact with a mock blog API. It includes endpoints for creating, retrieving, updating, and deleting blog posts, as well as fetching comments related to posts. The API supports various HTTP methods and query parameters to facilitate flexible data operations.

## Endpoints

### 1. Create a New Blog Post

- **Method:** `POST`
- **URL:** `/posts`
- **Description:**  
  Creates a new blog post. Provide required fields (such as `title`, `content`, and `author`) in the request body. Returns the details of the newly created post, including its unique `post_id`.

---

### 2. Retrieve All Blog Posts

- **Method:** `GET`
- **URL:** `/posts`
- **Description:**  
  Retrieves a list of all blog posts. Supports optional query parameters for filtering and pagination. Useful for displaying posts in a feed or dashboard.

---

### 3. Retrieve a Single Blog Post

- **Method:** `GET`
- **URL:** `/posts/{post_id}`
- **Description:**  
  Fetches the details of a single blog post identified by its unique `post_id`. Returns information such as the title, content, author, and other metadata.

---

### 4. Update a Blog Post (Full Update)

- **Method:** `PUT`
- **URL:** `/posts/{post_id}`
- **Description:**  
  Replaces an existing blog post with new data. The request body must contain the complete set of fields for the post. Any missing fields may be removed.

---

### 5. Update a Blog Post (Partial Update)

- **Method:** `PATCH`
- **URL:** `/posts/{post_id}`
- **Description:**  
  Partially updates a blog post. Only the fields provided in the request body will be updated. Useful for quick edits, such as updating the title or content.

---

### 6. Delete a Blog Post

- **Method:** `DELETE`
- **URL:** `/posts/{post_id}`
- **Description:**  
  Deletes a blog post identified by its unique `post_id`. This action is irreversible.

---

### 7. Retrieve Comments for a Post

- **Method:** `GET`
- **URL:** `/posts/{post_id}/comments`
- **Description:**  
  Retrieves comments associated with a specific blog post. Supports filtering and limiting results.

---

### 8. Retrieve All Comments

- **Method:** `GET`
- **URL:** `/comments`
- **Description:**  
  Retrieves all comments across all blog posts. Can be used to analyze feedback from users on various posts. Supports query parameters for advanced filtering.

---

## Usage

1. Import the collection into Postman using the provided link or JSON file.
2. Set the `baseURL` variable in your environment to point to your API server.
3. Use the endpoints as needed for development, testing, or demonstration purposes.

## Variables

- `baseURL`: The root URL for the API (e.g., `https://jsonplaceholder.typicode.com`)
- `post_id`: The unique identifier for a blog post

## License

This project is for demonstration and testing purposes.