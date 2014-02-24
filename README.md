# Canal.js

Canal.js is a lightweight JavaScript library for creating channels,
which are objects that represent a stream of events.

In the same way that [RSVP.js](https://github.com/tildeio/rsvp.js) is a
compact implementation of Promises/A+ that other library authors can use
to in their promise-based APIs, we intend library authors to use
Canal.js for the building blocks of their channel-based APIs. Hopefully,
this will allow for easy composition between channels created by
different libraries.

In keeping with the Unix philosophy, it is a modular library that does
one thing and does it well.

Building
---------

```sh
grunt
```

Development
-----------

The following will monitor your code, tests and vendored dependencies
and rebuild them as needed:

```sh
grunt server           # http://127.0.0.1:8000/
PORT=9292 grunt server # http://127.0.0.1:9292/
```

Testing
--------

```sh
grunt test         # headless testing (phantom + node)
grunt test:node    # node
grunt test:phantom # phantom
grunt server       # browser (navigate to http://127.0.0.1:8000)
```

Releasing
---------

- to bower (via github.com/components/<repo_name>)
- npm

```sh
grunt build-release release-it:0.0.1
```

Adding dependencies:
--------------------

- npm

```sh
npm install <package_name> --save     # runtime dependency
npm install <package_name> --save-dev # dev-dependency
```
