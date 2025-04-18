# Testing the Server

## Overview

<figure id="test-concept-map">
  <img src="test_concept_map.svg" alt="concept map of testing a server"/>
  <figcaption>Figure 1: Concept Map</figcaption>
</figure>

<p id="terms"></p>

## Outline

-   Add a [heartbeat](g:heartbeat) to [`server.py`](./server.py)
-   Wrap the [Flask][flask] application with a [test client](g:test-client)
    that provides an interface like [httpx][httpx]
-   Run `pytest test_heartbeat.py` to run tests in [`test_heartbeat.py`](./test_heartbeat.py)
-   Rewrite using [pytest][pytest] [fixtures](g:fixture) in [`test_fixtures.py`](./test_fixtures.py)
    -   Don't duplicate the expected value, since it might change
-   Patch database connection function in [`test_db.py`](./test_db.py) instead of creating a fixture
-   Use the two approaches together in [`test_combined.py`](./test_combined.py)
