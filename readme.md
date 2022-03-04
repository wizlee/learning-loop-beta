## 1️⃣ Overview

The original aim is to use Dotnet as the backend and Angular as the frontend. 
However, along the way also explored NextJS to learn more about its features.

### 📂 Folder List
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
- ⏮ Prerequisite
  - dotnet core installed
  - comfortable with command line OR install Visual Studio Community
- 🛠 Options
  - Using VS Code or any other lightweight IDE + command line
  - Or, download and install the latest Visual Studio Comunity edition

> The steps below will be using VS Code with the dotnet CLI only.
- 🏗 Steps for recreating this project
  1. `dotnet new angular -n DotnetAngularStripeExample -o dotnet-angular-stripe-example` 
    - It uses the angular template to create a dotnet core web project
    - Use `DotnetAngularStripeExample` as it's project name
    - Create the project inside a new folder called `dotnet-angular-stripe-example`
    - There are more options and available including [generating code for authentication](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity-api-authorization?view=aspnetcore-6.0).
      - Just need to append `-au Individual` to the dotnet new command. There are even [more advanced code generation](https://stackoverflow.com/questions/59927217/net-core-3-1-built-in-angular-spa-template-customize-login-register-template) by installing `dotnet-aspnet-codegenerator` tool.
      - However all that are redundant for the purpose of of this learning process.
    - We will remove the unused parts even from this minimal generated code in later steps.
  2. `cd dotnet-angular-stripe-example`
  3. The angular app that comes with the template is Angular 8, we are going to [upgrade it to Angular 12](https://www.freecodespot.com/blog/angular-with-dotnet-core-web-api/).
  4. To do that, we can either use [`ng update`](https://update.angular.io/?v=8.2-13.0) or recreate it using `ng new`. This project uses the later method.
  5. First, remove ClientApp folder by running `rm -rf ClientApp/`.
  6. Install Angular CLI globally by running `npm install -g @angular/cli`.
  7. Re-create the Angular App by running `ng new ClientApp --defaults=true --minimal=true`.
  8. Remove the following WeatherForecast controller related files. Also add an empty file called `.gitkeep` to keep the empty folder in source control.
    - WeatherForecast.cs
    - Controllers/WeatherForecastController.cs
  9. Run `dotnet run` to make sure everything is still working. You should see the default Angular welcome page.
  10. Profit 💰
    - Although all these steps are already completed in this repo, it will be valuable to go through it if you are not familar with aspnet core and Angular.
    - For example, [a reference to how the original Angular App fetch the mock weather data from the aspnet core](https://github.com/wizlee/learning-loop-beta/blob/4e25dcc1fec7e03ce4f0f3b433839972d84c022d/dotnet-angular-stripe-example/ClientApp/src/app/fetch-data/fetch-data.component.ts).
