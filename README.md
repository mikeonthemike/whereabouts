# where_is_api

WhereIsApi - JavaScript client for where_is_api
Find out where someone is
This SDK is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: class io.swagger.codegen.languages.JavascriptClientCodegen

## Installation

### For [Node.js](https://nodejs.org/)

#### npm

To publish the library as a [npm](https://www.npmjs.com/),
please follow the procedure in ["Publishing npm packages"](https://docs.npmjs.com/getting-started/publishing-npm-packages).

Then install it via:

```shell
npm install where_is_api --save
```

#### git
#
If the library is hosted at a git repository, e.g.
https://github.com/YOUR_USERNAME/where_is_api
then install it via:

```shell
    npm install YOUR_USERNAME/where_is_api --save
```

### For browser

The library also works in the browser environment via npm and [browserify](http://browserify.org/). After following
the above steps with Node.js and installing browserify with `npm install -g browserify`,
perform the following (assuming *main.js* is your entry file):

```shell
browserify main.js > bundle.js
```

Then include *bundle.js* in the HTML pages.

## Getting Started

Please follow the [installation](#installation) instruction and execute the following JS code:

```javascript
var WhereIsApi = require('where_is_api');

var api = new WhereIsApi.AdminsApi()

var teamMemberName = "teamMemberName_example"; // {String} pass a name in

var baseLocation = "baseLocation_example"; // {String} location to be set


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
api.updateBaseLocation(teamMemberName, baseLocation, callback);

```

## Documentation for API Endpoints

All URIs are relative to *https://virtserver.swaggerhub.com/mikeonthemike/whereIs/1.0.0*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*WhereIsApi.AdminsApi* | [**updateBaseLocation**](docs/AdminsApi.md#updateBaseLocation) | **POST** /location | updates base location
*WhereIsApi.DevelopersApi* | [**findTeamMember**](docs/DevelopersApi.md#findTeamMember) | **GET** /whereAbouts | searches whereabouts
*WhereIsApi.DevelopersApi* | [**searchLocation**](docs/DevelopersApi.md#searchLocation) | **GET** /location | searches locations
*WhereIsApi.DevelopersApi* | [**updateProjectLocation**](docs/DevelopersApi.md#updateProjectLocation) | **POST** /whereAbouts | updates location for a given team member and date


## Documentation for Models

 - [WhereIsApi.TeamMember](docs/TeamMember.md)
 - [WhereIsApi.Whereabouts](docs/Whereabouts.md)


## Documentation for Authorization

 All endpoints do not require authorization.

