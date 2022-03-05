## Authentication

Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

Authentication Solution and Sensitive Accounts
- Do NOT allow login with sensitive accounts (i.e. accounts that can be used internally within the solution such as to a back-end / middle-ware / DB) to any front-end user-interface
- Do NOT use the same authentication solution (e.g. IDP / AD) used internally for unsecured access (e.g. public access / DMZ)


- Password Length 
=>Minimum length=8 characters.
=>Maximum length= 64 characters .

Authentication and Error Messages:
- The user ID or password was incorrect.
- The account does not exist. 
- The account is locked or disabled.

### Basic access authentication:
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.Because the BA field has to be sent in the header of each HTTP request, the web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user for their username and password. Caching policy differs between browsers.

#### Client side Protocol
The Authorization header field is constructed as follows:
- The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
- The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified.
- The resulting string is encoded using a variant of Base64 (+/ and with padding).
- The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.

## Securing Passwords with Bcrypt Hashing Function
Cryptographic hash algorithms are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. 

There are some weaknesses in cryptographic hash algorithm that allows an attacker to calculate the original value of a hashed password:
PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM
- Brute Force attack: Hashes can't be reversed, so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack.
- Hash Collision attack


## node.bcrypt.js
A library to help you hash passwords.
Install via NPM:
npm install bcrypt

To hash a password:

Technique 1 (generate a salt and hash on separate function calls):
```
bcrypt.genSalt(saltRounds, function(err, salt) {
    bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {
        // Store hash in your password DB.
    });
});
```
Technique 2 (auto-gen a salt and hash):
```
bcrypt.hash(myPlaintextPassword, saltRounds, function(err, hash) {
    // Store hash in your password DB.
});
```

To check a password:
```
// Load hash from your password DB.
bcrypt.compare(myPlaintextPassword, hash, function(err, result) {
    // result == true
});
bcrypt.compare(someOtherPlaintextPassword, hash, function(err, result) {
    // result == false
});
```
[Home](./README.md)<br>
