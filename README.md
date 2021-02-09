# [Build an app with ASPNET Core and Angular from scratch](https://www.udemy.com/course/build-an-app-with-aspnet-core-and-angular-from-scratch/)

## Table of contents
- [Build an app with ASPNET Core and Angular from scratch](#build-an-app-with-aspnet-core-and-angular-from-scratch)
  - [Table of contents](#table-of-contents)
  - [General info](#general-info)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Run](#run)

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