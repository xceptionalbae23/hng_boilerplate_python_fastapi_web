 # HNG_STAGE_3_TASK

The  API provides endpoints to manage users, organizations, posts, and payments, with features such as registration, login, adding users to organizations, creating posts, and managing payments through various providers.
FastAPI boilerplate

## Setup

## DESCRIPTION

Click the link below, TO access the  API Design Documentation


[API Design](https://unyimeudemy.github.io/HNG_API_page/)

## API Reference

#### GET ALL USERS

```http
  GET /api/users

```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `user` | `string` | **Required**. ID of the user to fetch |

#### Get userId

```http
  GET /api/user/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `userId`      | `string` | **Required**. Id of users to fetch |

#### Create user

```http

  POST /api/users
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `user`      | `string` | **Required**. Id to add users  |


#### ORGANIZATION

#### Get all organizations

```http

   GET /api/organisations

```
Retrieve a list of all organizations.

Get organization by ID

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `orgId`      | `string` | **Required**. ID of the organization to fetch  |

Create organization
```http
  POST /api/organisations
```

Create a New organisations

Get Users in the organization
```http
  GET /api/organisations/${orgId}/users

```



| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `orgId`      | `string` | **Required**. ID of the organization to fetch users from |

Add Users to Organisations
```http
  POST /api/organisations/${orgId}/users

```
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `orgId`      | `string` | **Required**. ID of the organization to add users to |

Get organisations for Users
```http
  GET /api/organisations/${userId}/organisations

```
| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `userId`      | `string` | **Required**.  ID of the user to fetch organizations for |


**POST**


Get all Post
```http
  GET /api/posts

```

Retrieve a list of all posts.

Get post by ID
```http
  GET /api/posts/${postId}

```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `postId`      | `string` | **Required**.  ID of the post to fetch  |

Create Post
```http
  POST /api/posts

```
Create a new post

**PAYMENTS**

Create payment with Stripe
```http
  POST /api/payments/stripe

```
Get all payments
```http
  GET /api/payments

```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `postId`      | `string` | **Required**.  ID of the post to fetch  |




## Installation

Clone the repository:

```bash
git clone  git clone https://github.com/xceptionalbae23/hng_boilerplate_python_fastapi_web.git

cd hng_boilerplate_python_fastapi_web


```



```bash
psql -
CREATE DATABASE IMAGE;
<a>
    <img height="600px" src="https://solididbucket.s3.amazonaws.com/HNG+Boilerplate.png" alt="Jenkins logo"> 
</a>





Build and run the application:
```bash
mvn clean install
mvn spring-boot:run


```
Access the Swagger UI to interact with the API:
```bash




```











1. Create a virtual environment.
 ```sh
    python3 -m venv .venv
 ```
2. Activate virtual environment.
```sh
    source /path/to/venv/bin/activate`
```
3. Install project dependencies `pip install -r requirements.txt`
4. Create a .env file by copying the .env.sample file
`cp .env.sample .env`

5. Start server.
 ```sh
 python main.py
```

