* Introduction to JSON Web Tokens [Link](https://jwt.io/introduction/)
  * _Signed_ JWTs guarantee authenticity while _encrypted_ JWTs ensure the information is hidden.
  * JWTs are useful for authorization as it allows access to be obtained by the right parties.
  * JWTs can be used for data exchange to ensure information is not tampered with from sender to recipient.
  * JWTS consists of a header, payload, and signature with the structure xxxxx.yyyyy.zzzzz.
  * The header contains the type of signing algorithm and the type of the token. Example:
  ```
  {
  "alg": "HS256",
  "typ": "JWT"
  }
  ```
  * The payload contains the claims (information). These can be registered, public, or private claims. Example:
  ```
  {
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
  }
  ```
  * The signature is created from an encoded header, payload, and secret using the algorithm specified in the header. Example:
  ```
  HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
  ```
  * After it is Base64 encrypted the JWT will look like:
  ```
  eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
  ```
  * JWT is more compact than other tokens and thus reaps a lot of efficiency benefits.

* Why You Should Use BCrypt To hash passwords [Link](https://danboterhoven.medium.com/why-you-should-use-bcrypt-to-hash-passwords-af330100b861)
  * Hashed passwords are preferable to plain text because they are less common and often not duplicated across applications.
  * One way hash is slightly more secure but it can still be accessed by brute force guessing.
  * Salting a passwords add a secret bit of text onto a user's password so a hacker would need access to the source code to figure this out.
  * Random salt is similar but changes the appended text each time.
  * BCrypt uses a key factor to slow down hashing speeds to stop brute force hack attacks.

* Hashing In Action: Understanding BCrypt [Link](https://auth0.com/blog/hashing-in-action-understanding-bcrypt/)
  * One downside to using SHA is that because it is fast, hackers can try more passwords per second in a brute force attack.
  * As hardware becomes more powerful it will become faster for hackers to exploit a fast algorithm. By being able to slow the algorithm over time removes that advantage to the hacker.
  * BCrypt uses a 128-bit salt and 192-bt magic value to create a stronger password.
  * BCrypt runs in two phases:
    * Setup Phase: initializes salt, cost, keys schedule, etc.
    * Operation Phase: Using the magic and salt values the password is then encrypted 64 times.
  * Can use two-factor authentication on top of bcrypt to make passwords more secure.
  * There is a built in library in Node.js that allows bcrypt to be used easily.

