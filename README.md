## MUST DO THIS BEFORE RUN

## CREATE ANGULAR PROJECT WITH LOCAL CLI

npx -p @angular/cli ng new `<project-name>`
npx @angular/cli@7 new Angular7Project

https://medium.com/@starikovs/how-to-use-angular-cli-locally-729dbb6707dd

---

# INSTALL ALL THESE

npx -p @angular/cli ng new `<project-name>`

npm i @angular/material@12.2

npm install --save @angular/cdk@12.2

npm start

---

# CREATE COMPONENT

ng generate component banner --skipTests true --modile app.module.ts

npm run ng generate component banner --skipTests true --module app.module.ts

# CREATE COMPONENT [WHEN PROJECT GENERATED WITH LOCAL CLI]

npm run ng -- generate component banner --module=app

# if browser console give error

`ERROR Error: Unexpected synthetic property @transitionMessages found. Please make sure that:`

Import this in `app.module.ts` register it imports
import { BrowserModule } from '@angular/platform-browser';

`@NgModule({ ..., imports: [ ..., BrowserAnimationsModule ], ... })`

## Add Material Icon

`<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`

## OR

`@import url("https://fonts.googleapis.com/icon?family=Material+Icons");`

# Run

`npm start` or `yarn start`
