# [Build an app with ASPNET Core and Angular from scratch](https://www.udemy.com/course/build-an-app-with-aspnet-core-and-angular-from-scratch/)

## Table of contents

- [Build an app with ASPNET Core and Angular from scratch](#build-an-app-with-aspnet-core-and-angular-from-scratch)
  - [Table of contents](#table-of-contents)
  - [General info](#general-info)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Run](#run)
  - [Tips](#tips)

## General info

> A practical example of how to build an application with ASP.NET Core API (.Net 5.0) and Angular 10 from start to finish by buiding application named Dating App

## Prerequisites

* [Dotnet core 5.0](https://dotnet.microsoft.com/download/dotnet/5.0)
* [Angular](https://angular.io/)
* Cloundinary API

## Setup

1. Install dotnet
2. Check dotnet by typing 
```bash
dotnet --version
```
3. Install npm
4. Install angular cli
```bash
npm install -g @angular/cli@11.2.13
```
5. Config cloudinary section in appsettings.json
```js
"CloudinarySettings": {
  "CloudName": "Your cloud Name",
  "ApiKey": "Your api key",
  "ApiSecret": "Your api secret"
}
```

## Run

* API
```bash
cd API/
dotnet restore
dotnet run
```
* client
```bash
cd client/
ng serve
```

## Tips

* If you encounter line below while running **ng serve**  
   ```bash
   An unhandled exception occurred: cannot find module '@angular-devkit/build-angular/package.json'
   ```   
   please goto client directory and type below command in terminal
   ```bash
   ng version
   ```
   **Result**
   ```bash
    Package                         Version
    ---------------------------------------------------------  
    @angular-devkit/architect       0.1102.13 (cli-only)       
    @angular-devkit/build-angular   <error>
    @angular-devkit/core            11.2.13 (cli-only)
    @angular-devkit/schematics      11.2.13 (cli-only)
    @angular/cli                    11.2.13 (cli-only)
    @schematics/angular             11.2.13 (cli-only)
    @schematics/update              0.1102.13 (cli-only)
    rxjs                            6.6.3 (cli-only)
    typescript                      <error>
   ```
   Then run this command to install **@angular-devkit/build-angular** and **typescript**
   ```bash
   npm i --save-dev @angular-devkit/build-angular@0.1102.13
   npm i --save-dev typescript@4.1.5
   ```
