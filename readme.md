## Overview

> This repo is to document all learning process during the first week of the Learning Loop program.

The original aim is to use Dotnet as the backend and Angular as the frontend. However, along the process also explored NextJS to learn more about its features.

### Folder List
Try to contained each learning inside a folder. Below are the brief description for each of them.
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
  3. The angular app that comes with the template is Angular 8, we are going to [upgrade it to Angular 12](https://www.freecodespot.com/blog/angular-with-dotnet-core-web-api/).
  4. To do that, we can either use [`ng update`](https://update.angular.io/?v=8.2-13.0) or recreate it using `ng new`. This project uses the later method.
  5. First, remove ClientApp folder by running `rm -rf ClientApp/`.
  6. Re-create the Angular App by running `ng new ClientApp --defaults=true --minimal=true`.
  7. TBC...
  