# html5-boilerplate

Simple web application that uses the standard HTML5 boilerplate.


## Running Locally

```html
> npm install

> npm start

```

Should open the server as http://localhost:1234/


## Hosting

This web site is hosted on Azure using [Static Web Apps](https://azure.microsoft.com/en-us/services/app-service/static/) service. When a change is made to the code and it is uploaded onto Git, the code is automatically compiled and uploaded to Azure. A log of all 
the compiles are stored on GitHub [here](https://github.com/liam-grossmann/html5-boilerplate/actions?query=workflow%3A%22Azure%20Static%20Web%20Apps%20CI%2FCD%22%20branch%3Amain)

Static web pages are free to host on Azure. They are the perfect way to showcase your front end coding skills.

The site is hosted as https://proud-mud-0ab2c3803.2.azurestaticapps.net.


## Changelog and Fixes

Removed most npm warnings and errors
* Upgraded from parcel-budler v1.2 to parcel v2.0. See [here](https://parceljs.org/getting-started/migration/) for more.
* Added the engines setting to package.json to fix Azure build failures. The 'engines' tag specifies node and npm versions.
* Added @parcel/transformer-webmanifest and some other parcel libraries as dev dependancies to fix some Azure build errors.


NOTE:
Some warnings cannot be fixed. Parcel v2 has dependancies on some deprecated packages. The solution might be to use Webpack.
* npm WARN deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility

