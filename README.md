# password-storage
Java Sample program for Password Storage 

Program uses HMAC-SHA-256 as the core hash inside PBKDF2.

It creates hash in format : algorithm:iterations:hashSize:SALT:hash for demonstration purpose. We can store salt and actual hash in table which will be unique for each users.

Everytime user create it's password, system will generate a new SALT and HASH. Number of iteration can be calculated based on concurrent load on your authentication server at peak time.

We are using PBKDF2 algorithm to generate password hash.


