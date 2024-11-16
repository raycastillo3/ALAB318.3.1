# Node.js
This is a Node.js project.

## ROUTES:
Clone repository, run these endpoints on your local host: 

GET /api/users/:id/posts
Retrieves all posts by a user with the specified id.

http://localhost:3000/api/users/1/posts?api-key=perscholas 

GET /api/posts?userId=<VALUE>
Retrieves all posts by a user with the specified postId.

http://localhost:3000/api/posts?userId=1&api-key=perscholas

GET /comments

http://localhost:3000/api/comments?api-key=perscholas

POST /comments
It should have the following fields: 
* __id__: a unique identifier. 
* __userId__: the id of the user that created the comment.
* __postId__: the id of the post the comment was made on.
* __body__: the text of the comment.

http://localhost:3000/api/comments?api-key=perscholas

GET /comments/:id
Retrieves the comment with the specified id.

http://localhost:3000/api/comments/1/?api-key=perscholas

PATCH /comments/:id
Used to update a comment with the specified id with a new body.

http://localhost:3000/api/comments/1/?api-key=perscholas

DELETE /comments/:id
Used to delete a comment with the specified id.
Make sure you use an id that is valid or make a POST request first
http://localhost:3000/api/comments/1/?api-key=perscholas

GET /comments?userId=<VALUE>
Retrieves comments by the user with the specified userId.

http://localhost:3000/api/comments?userId=1&api-key=perscholas

GET /comments?postId=<VALUE>
Retrieves comments made on the post with the specified postId.

http://localhost:3000/api/comments?postId=1&api-key=perscholas

GET /posts/:id/comments
Retrieves all comments made on the post with the specified id.

http://localhost:3000/api/posts/1/comments?api-key=perscholas

GET /users/:id/comments
Retrieves comments made by the user with the specified id.

http://localhost:3000/api/users/1/comments?api-key=perscholas

GET /posts/:id/comments?userId=<VALUE>
Retrieves all comments made on the post with the specified id by a user with the specified userId.

http://localhost:3000/api/users/1/comments?postId=1&api-key=perscholas

GET /users/:id/comments?postId=<VALUE>
Retrieves comments made by the user with the specified id on the post with the specified postId.

http://localhost:3000/api/users/1/comments?postId=1&api-key=perscholas