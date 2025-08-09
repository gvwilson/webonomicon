# Encryption

## Overview

<figure id="crypt-concept-map">
  <img src="crypt_concept_map.svg" alt="concept map of password encryption"/>
  <figcaption>Figure 1: Concept Map</figcaption>
</figure>

## Outline

-   Never store passwords as [plaintext](g:plaintext)
-   Create a migration to encrypt them and save [ciphertext](g:ciphertext)
    -   Generate a [secret](g:secret) in [`generate_encryption.py`](./generate_encryption.py)
    -   `make_secret` in [`util.py`](./util.py) uses Python's [secrets][secrets] module
    -   Save in a file that never goes in version control (or anywhere else)
    -   Then encrypt passwords using `blake2b` from [hashlib][hashlib]
-   [Hash](g:hashing) the combination of the secret and their password
    -   The secret is a [salt](g:salt)
-   When someone logs in:
    -   Check that the encrypted version of the secret plus their password matches the stored value
    -   Create a random number as a cookie
    -   Store that and their ID in a dictionary of [sessions](g:session)
-   When someone requests access to experimental data:
    -   If their cookie is in the sessions, use their staff ID
    -   Otherwise reject as unauthorized
-   Still insecure
    -   We are getting their password over an unencrypted channel
    -   The cookie is being passed back and forth over the same channel
    -   Look at certificates in [an appendix](../99_cert/)
