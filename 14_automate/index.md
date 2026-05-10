# Testing in the Browser

<p id="terms"></p>

## Overview

[% figure slug="test-concept-map" img="test_concept_map.svg" alt="concept map of browser-based testing" caption="Figure 1: Concept Map" %]

## Outline

-   [%g browser-automation "Automate the browser" %] with [Selenium][selenium]
-   [`test_home_page.py`](./test_home_page.py)
    -   Create a driver in a fixture that uses `yield` to ensure shutdown
    -   Go to a URL
    -   Inspect elements
-   [`test_login.py`](./test_login.py) interacts with the browser
    -   Find elements
    -   Simulate typing and button clicking
    -   Wait for the browser to update
    -   Check the cookie is present
