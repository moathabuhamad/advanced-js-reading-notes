### What header(s) are used in authentication and authorization
Basic Auth
Bearer Token
Digest Auth
and many other


### What is safe to put into a JWT
JWT are not encrypted by default, so care must be taken with the information included inside the token. If you need to include sensitive information inside a token, then encrypted JWT must be used.

### How are JWTs validated
JWTs have a secret key, When the client receives token, the client uses the same key

|Terms|Defenition|
|---|---|
|RBAC|Role-Based Access Control, defines roles and privileges.|
|JSON web token (JWT)|pronounced "jot", is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. Again, JWT is a standard, meaning that all JWTs are tokens, but not all tokens are JWTs.|
|
