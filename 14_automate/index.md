# Testing in the Browser

## Overview

<figure id="test-concept-map">
  <img src="test_concept_map.svg" alt="concept map of browser-based testing"/>
  <figcaption>Figure 1: Concept Map</figcaption>
</figure>

<p id="terms"></p>

## Outline

-   [Automate the browser](g:browser-automation) with [Selenium][selenium]
    -   [This tutorial][selenium-tutorial] is helpful
-   [`test_home_page.py`](./test_home_page.py)
    -   Create a driver in a fixture that uses `yield` to ensure shutdown
    -   Go to a URL
    -   Inspect elements
-   [`test_login.py`](./test_login.py) interacts with the browser
    -   Find elements
    -   Simulate typing and button clicking
    -   Wait for the browser to update
    -   Check the cookie is present
