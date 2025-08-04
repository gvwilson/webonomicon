# The Webonomicon

<p class="subtitle">An Introduction to Web Programming for the Cautious and Weary</p>

This tutorial is a short introduction to web programming using modern tools and practices
for data scientists who are comfortable using Python
but have never built interactive websites before.
All of the material is available under [open licenses](./LICENSE.md),
and contributions through our [GitHub repository][repo] are welcome.
All contributors are required to respect our [Code of Conduct](./CODE_OF_CONDUCT.md).

> **Please note:** this tutorial is still being outlined.
> Most sections will have additional examples (and much more explanation)
> before learners encounter it.
> Suggestions and help are greatly appreciated.

## Learner Persona

-   Sabina, 28, has a master's degree in animal physiology
    and now works for a mid-sized veterinary pharmaceutical company.
-   She learned a bit of R in an undergraduate biostatistics course,
    then picked up Python in grad school.
    She spends several hours a week analyzing data with [Pandas][pandas]
    and visualizing it with [Plotly Express][plotly-express],
    and is comfortable with basic Git commands.
-   Sabina recently became responsible for maintaining a dashboard application built with [Dash][dash].
    She believes a better understanding of how web applications work in general
    will help her debug and extend it.
-   Sabina has tried doing asynchronous online courses a couple of times,
    but strongly prefers learning in real time with other people.

## Syllabus

<div id="syllabus" markdown="1">

1.  [Introduction](./01_intro/): what we will learn, how to set up, and the data we will use
1.  [HTML and CSS](./02_htmlcss/)
1.  [An Hour of JavaScript](./03_js/)
1.  [JavaScript in the Browser](./04_browser/): using the language in its native habitat
1.  [HTTP](./05_http/): how browsers and server talk to each other
1.  [A Server](./06_server/): building a server with [Flask][flask]
1.  [Using a Database](./07_db/): getting data from [SQLite][sqlite] using [PyPika][pypika]
1.  [Testing the Server](./08_test/): testing the server with [pytest][pytest]
1.  [Serving HTML](./09_view/): generating HTML with [Jinja][jinja] templates
1.  [Using Forms](./10_forms/): sending data to a server
1.  [Using HTMX](./11_htmx/): letting the [htmx][htmx] library do the hard work
1.  [Database Migration](./12_migrate/): managing database schema changes
1.  [Authentication](./13_auth/): checking the user's identity
1.  [Testing in the Browser](./14_automate/): using [Selenium][selenium] to test the user interface
1.  [Encryption](./15_crypt/): keeping secrets safe
1.  [Uploading Files](./16_upload/): multi-step interactions
1.  [Logging and Auditing](./17_log/): keeping of track of what's happened
1.  [Permissions](./18_perm/): representing and checking who can do what
1.  [Accessibility](./19_access/): because everyone should be comfortable
1.  [A Graphical User Interface](./20_gui/): handling interactivity in the browser
1.  [Dynamic Graphics](./21_graphics/): drawing pictures with [SVG.js][svgjs]
1.  [Internationalization](./22_intl/): because everyone should be welcome
1.  [Sessions](./23_sessions/): persistent sessions and [JWT][jwt]
1.  [Caching](./24_cache/): speeding things up

</div>

##  Appendices

<div id="appendices" markdown="1">

1.  [Designing a Workflow](./98_workflow/)
1.  [Certificates](./99_cert/)
1.  [License](./LICENSE.md)
1.  [Code of Conduct](./CODE_OF_CONDUCT.md)
1.  [Bibliography](./bibliography.md)
1.  [Glossary](./glossary.md)

</div>

<p class="center">
  <em>
    Start where you are
    <br/>
    Use what you have
    <br/>
    Help who you can
  </em>
</p>

[alpine]: https://alpinejs.dev/
[bs4]: https://beautiful-soup-4.readthedocs.io/
[dash]: https://dash.plotly.com/
[deno]: https://deno.com/
[fasthtml]: https://docs.fastht.ml/
[flask]: https://flask.palletsprojects.com/
[frappe-charts]: https://frappe.io/charts/docs
[html5validator]: https://pypi.org/project/html5validator/
[htmx]: https://htmx.org/
[httpx]: https://www.python-httpx.org/
[jinja]: https://jinja.palletsprojects.com/
[jwt]: https://en.wikipedia.org/wiki/JSON_Web_Token
[pandas]: https://pandas.pydata.org/
[plotly-express]: https://plotly.com/python/plotly-express/
[polars]: https://pola.rs/
[prettytable]: https://pypi.org/project/prettytable/
[pypika]: https://pypika.readthedocs.io/
[pytest]: https://docs.pytest.org/
[repo]: https://github.com/gvwilson/webonomicon
[selenium]: https://pypi.org/project/selenium/
[sqlite]: https://www.sqlite.org/
[svgjs]: https://svgjs.dev/
