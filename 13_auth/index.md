# Authentication

<p id="terms"></p>

## Overview

[% figure slug="auth-concept-map" img="auth_concept_map.svg" alt="concept map of authentication" caption="Figure 1: Concept Map" %]

## Outline

-   Assign everyone staff member a user ID and a 4-digit PIN
-   Generate account data with [`generate_accounts.py`](./generate_accounts.py)
    -   Use a [Jinja][jinja] template to produce a SQL file for migration
    -   Doesn't check for uniqueness of generated usernames
-   [`server.py`](./server.py)
    -   Set the user's staff ID as the [%g cookie "cookie" %]
    -   Horribly insecure (easy to fake)
    -   Only show experiments to the person who created them
    -   Handling cookies in JavaScript (or Python) is unpleasant
