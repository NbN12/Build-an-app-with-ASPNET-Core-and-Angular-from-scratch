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
> A practical example of how to build an application with ASP.NET Core API (.Net 5.0) and Angular 10 from start to finish

## Prerequisites
* [Dotnet core 5.0](https://dotnet.microsoft.com/download/dotnet/5.0)
* [Angular](https://angular.io/)

## Setup
1. Install dotnet
2. Check dotnet by typing 
```bash
dotnet --version
```
3. Install npm
4. Install angular cli
```bash
npm install -g @angular/cli@10.2.0
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
   please check your **ng cli** by typing this command.
   ```bash
   ng version
   ```
   **Result**
   ```bash
   Package                         Version
   ---------------------------------------------------------
   @angular-devkit/architect       0.1002.0 (cli-only)
   @angular-devkit/build-angular   <error>              (show no package here)
   @angular-devkit/core            10.2.0 (cli-only)
   @angular-devkit/schematics      10.2.0 (cli-only)
   @angular/cli                    10.2.0 (cli-only)
   @schematics/angular             10.2.0 (cli-only)
   @schematics/update              0.1002.0 (cli-only)
   rxjs                            6.6.2 (cli-only)
   typescript                      <error>              (show no package here)
   ```
   Then run this command to install **@angular-devkit/build-angular** and **typescript**
   ```bash
   npm i --save-dev @angular-devkit/build-angular
   npm i --save-dev typescript
   ```
