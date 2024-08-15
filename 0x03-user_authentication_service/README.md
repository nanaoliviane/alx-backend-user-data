# 0x03. User authentication service
## Back-end
## Authentification


# Setup
You will need to install bcrypt

pip3 install bcrypt

# User model
In this task you will create a SQLAlchemy model named User for a database table named users (by using the mapping declaration of SQLAlchemy).

The model will have the following attributes:

id, the integer primary key
email, a non-nullable string
hashed_password, a non-nullable string
session_id, a nullable string
reset_token, a nullable string

# 1. create user
In this task, you will complete the DB class provided below to implement the add_user method.
Note that DB._session is a private property and hence should NEVER be used from outside the DB class.

Implement the add_user method, which has two required string arguments: email and hashed_password, and returns a User object. The method should save the user to the database. No validations are required at this stage.

