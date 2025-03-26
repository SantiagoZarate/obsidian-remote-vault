There are a lot of SHA (Security Hashing Algorithm), the difference between SHA-1 and SHA-256 are:

| Algo    | Output Size         | Strength                                                                                                                |
| ------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| SHA-1   | 160 bit (20 bytes)  | Considered weak and broken (vulnerable to collisions since 2005; fully practical collisions were demonstrated in 2017). |
| SHA-256 | 256 bits (32 bytes) | Much stronger, part of the SHA-2 family; still considered secure and used in modern security protocols.                 |

## **Collision resistance**

**SHA-1** has known collisions (two different inputs producing the same output).

**SHA-256** has no known collisions and is designed to be far more resistant to them.

## **Recommendation**

If the API allows it, **always go for `HMAC-SHA256`** for better security.

If you’re integrating with legacy systems or APIs that don’t support it, you might be forced to use `HMAC-SHA1`.

*SHA-256 is used in things like Bitcoin or HTTPS!*

