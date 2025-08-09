# Introduction

-   Sooner or later you're going to want to share your findings
-   And learning how the web works is fun
-   Use modern Python and JavaScript tools
    -   Yes, you're going to have to learn some JavaScript…
    -   …but it's not as bad as you've been told
-   All of these materials can be freely re-used under an [open license](@root/license/)

## Setup

-   Install [uv][uv] for managing Python packages and [virtual environments](g:virtual-env) and then run:
    -   `uv venv` in the root directory of this project to create a virtual environment in `./.venv`
    -   `source .venv/bin/activate` to activate that virtual environment
    -   `uv pip install -r pyproject.toml` to install requirements
-   To regenerate the sample data, run `make datasets` to:
    -   install the default parameters for `snailz` in `./params`, and
    -   regenerate the sample data in `./data`
    -   We use [Make][make] to run tasks because every other option proved to be more complicated
-   Project uses [McCole][mccole] to generate and check HTML
    -   Run `make render` to regenerate the HTML in `./docs` from the Markdown files
    -   Run `make lint` at any time to check the state of the project

## The Data

[snailz][snailz] creates synthetic data for a study of mutant snails in the Pacific Northwest.

-   One or more *surveys* are conducted at one or more *sites*.
-   Each survey collects *genomes* and *sizes* of snails.
-   A *grid* at each site is marked out to show the presence or absence of pollution.
-   *Staff* perform *assays* of the snails' genetic material.
-   Each assay plate has a *design* showing the material applied and *readings* showing the measured response.
-   Plates may be *invalidated* after the fact if a staff member believes it is contaminated.

## Technologies

| Package                          | Purpose           |
| -------------------------------- | ----------------- |
| [Alpine.js][alpine]              | dynamic HTML      |
| [Beautiful Soup][bs4]            | HTML manipulation |
| [deno][deno]                     | JavaScript        |
| [FastHTML][fasthtml]             | web framework     |
| [Flask][flask]                   | web server        |
| [Frappe Charts][frappe-charts]   | charts            |
| [html5validator][html5validator] | validation        |
| [htmx][htmx]                     | interaction       |
| [httpx][httpx]                   | HTTP              |
| [Jinja2][jinja]                  | HTML templating   |
| [Polars][polars]                 | tabular data      |
| [PrettyTable][prettytable]       | formatting        |
| [PyPika][pypika]                 | query builder     |
| [pytest][pytest]                 | testing           |
| [Selenium][selenium]             | testing           |
| [SQLite][sqlite]                 | database          |
| [SVG.js][svgjs]                  | graphics          |

## Acknowledgments {: #acknowledgments}

-   Grateful to co-authors of [[Gans2020](b:Gans2020)]
-   And to everyone who gave feedback on [[Wilson2022](b:Wilson2022), [Wilson2024](b:Wilson2024)]

[alpine]: https://alpinejs.dev/
[bs4]: https://beautiful-soup-4.readthedocs.io/
[deno]: https://deno.com/
[fasthtml]: https://docs.fastht.ml/
[flask]: https://flask.palletsprojects.com/
[frappe-charts]: https://frappe.io/charts/docs
[html5validator]: https://pypi.org/project/html5validator/
[htmx]: https://htmx.org/
[httpx]: https://www.python-httpx.org/
[jinja]: https://jinja.palletsprojects.com/
[make]: https://www.gnu.org/software/make/
[mccole]: https://gvwilson.github.io/mccole/
[polars]: https://pola.rs/
[prettytable]: https://pypi.org/project/prettytable/
[pypika]: https://pypika.readthedocs.io/
[pytest]: https://docs.pytest.org/
[selenium]: https://pypi.org/project/selenium/
[snailz]: https://gvwilson.github.io/snailz/
[sqlite]: https://www.sqlite.org/
[svgjs]: https://svgjs.dev/
[uv]: https://docs.astral.sh/uv/
