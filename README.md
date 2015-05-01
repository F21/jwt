JWT
===
A PHP library for encoding and decoding JSON Web Tokens.

**Important security notice**

Thanks to Toshiharu Sugiyama!

Please upgrade to 2.0 as soon as possible as previous versions are susceptible to verification bypass attacks if the same public key is used for signing when using asymmetric and symmetric algorithms.

This is a release breaks backwards compatibility because you now need to pass in the decoding algorithm when decoding in order to verify the JWT.

For more information see: JVN#06120222 at jpcert.or.jp


Supported Algorithms
--------------------

**HMAC**

* HS256	- HMAC using SHA-256 hash algorithm (default)
* HS384	- HMAC using SHA-384 hash algorithm
* HS512 - HMAC using SHA-512 hash algorithm

**RSA (Public Key/Private Key pair)**

* RS256 - RSA using SHA-256 hash algorithm
* RS384 - RSA using SHA-384 hash algorithm
* RS512 - RSA using SHA-512 hash algorithm