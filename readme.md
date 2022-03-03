## Overview

This repo contains several exploratory projects and tools

### Project List
- `checkout-one-time-payment` is a sample created by using stripe CLI
  - it uses vanilla html as FE, dotnet as BE
- `dotnet-vanilla-html-stripe-example` is a sample downloaded directly from [stripe quickstart page](https://stripe.com/docs/checkout/quickstart)
  - it uses vanilla html as FE, dotnet as BE
- `nextjs-prebuilt-checkout` is a sample downloaded directly from [stripe quickstart page](https://stripe.com/docs/checkout/quickstart)
  - it uses nextjs as both the FE and BE
- `postman-to-vscode-rest-client` is a tool from [this github repo](https://github.com/alfathdirk/postman-to-vscode-rest-client)
  - this is used to convert postman collection into .http files used by vscode rest client extensions.
- `http-request` contains .http files that are used for quick development testing of various HTTP APIs.
- `dotnet-angular-stripe-example` is a sample created from scratch
  - Refer to the [Dotnet Angular Example section](#dotnet-angular-example) below for more details.

### Dotnet Angular Example
- Prerequisite
  - dotnet core installed
  - comfortable with command line OR install Visual Studio Community
- Options
  - Using VS Code or any other lightweight IDE + command line
  - Or, download and install the latest Visual Studio Comunity edition
- Steps for recreating this project
  1. `dotnet new angular -n DotnetAngularStripeExample -o dotnet-angular-stripe-example` 
    - it uses the angular template to create a dotnet core web project
    - Use `DotnetAngularStripeExample` as it's project name
    - Create the project inside a new folder called `dotnet-angular-stripe-example`
  2. `cd dotnet-angular-stripe-example`
  3. TBC
