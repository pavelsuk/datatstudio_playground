# Datastudio Playground

How to's and code snippets for integration with Google datastudio

## Sources

- [Connectors](https://developers.google.com/datastudio/connector/)
- [Get Started](https://developers.google.com/datastudio/connector/get-started)
- [CodeLab example](https://codelabs.developers.google.com/codelabs/community-connectors/#0)
- [Apps Script Home Page](https://script.google.com/home)
    - [Developing Apps script locally](https://codelabs.developers.google.com/codelabs/clasp/#0)
- [API reference](https://developers.google.com/datastudio/connector/reference)
- [Community Connectors on Github](https://github.com/googledatastudio/community-connectors)
    - [NPM Downloads example](https://github.com/googledatastudio/community-connectors/tree/master/npm-downloads)

## Developing Apps script locally

- Install: `npm i @google/clasp -g`
- Login: `clasp login`

### Create test application

``` bash
mkdir clasp_codelab
cd clasp_codelab
clasp create "Clasp Codelab"
```

#### Optionally: Clone Existing Project

``` bash
clasp clone <scriptID>
```

where `scriptID` is found in [script.google.com](https://script.google.com/home) under **File > Project properties > Info > Script ID** or in the URL for particular script

### Edit it

- Online: `clasp open`
- Locally: `clasp pull`, `clasp push`

### Versioning

See [Tutorial](https://codelabs.developers.google.com/codelabs/clasp/#5)

``` bash
clasp version "First version"
clasp deploy 1 "First deployment"
```

## Important Files for Datastudio connector

Cloned from [NPM Downloads example](https://github.com/googledatastudio/community-connectors/tree/master/npm-downloads):

- [manifest: clasp_codelab/appsscript.json](clasp_codelab/appsscript.json)
- [script: clasp_codelab/Code.js](clasp_codelab/Code.js)

## Difference between dimensions and metrics

_[Source: About dimensions and metrics](https://support.google.com/datastudio/answer/6402048?hl=en&ref_topic=7441655)_

> Fields contain the information that appears in your reports. There are 2 types of fields in a data source: **dimensions** and **metrics**.
> 
> A dimension is a category of data, while a metric is a number that quantifies something in that category. When you add a data source to a report, its fields become available for use in charts and controls.