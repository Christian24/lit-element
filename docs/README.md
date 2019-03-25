## lit-element Documentation 

This folder holds the source for the lit-element documentation site. Guides are written in Markdown, and the site is built using the Jekyll static site generator. 
 
This section describes how to build the documentation site.

### Prerequisites

To build the documentation site, you need Jekyll, Node, npm, and Polymer CLI.

If you already have Ruby and the gem pacakge manager, run the following command to install Jekyll:

`gem install bundler jekyll`

For more information, see [the Jekyll website](https://jekyllrb.com/).

To install Polymer CLI: 

`npm install -g polymer-cli`

Previewing the docs requires the [App Engine Standard Environment for Python 2.7](https://cloud.google.com/appengine/docs/standard/python/quickstart). 

### Setup

1. Clone or download a copy of this repo.

2. Install npm dependencies for the docs site.

    ```
    cd lit-element/docs
    npm install
    ```

### Building and previewing

To build the documentation site and preview it from a local server:

```
cd docs
npm run build
npm run serve
```

Point a browser at [localhost:8080](localhost:8080) to preview the site.
To use a different port, run:

```
npm run serve -- --port <PORTNUMBER>
```

The generated API docs are checked in, so you don't need to build the 
API docs unless you're making changes to the doc comments in the lit-element source.

To regenerate the API docs and rebuild the  site, run the following command:

`npm run build-all`
