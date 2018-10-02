[![Build Status](https://app.codeship.com/projects/795fc650-a62b-0136-a66a-2ac20198919e/status?branch=master)]

# Deploy your Angular app on Google Kubernetes Engine(GKE) with the help of docker tarvis nginx

create Angular App

```ng new your-app-name```

Build your app for production

```ng build --prod ```

# Write DockerFile for Angualr App

   ```
      FROM nginx:1.13
      COPY  dist/ /usr/share/nginx/html
      EXPOSE 80
   ```
      
"From nginx:1.13" it means that we are taking the nginx image from dockerhub, "COPY  dist/ /usr/share/nginx/html" it means that we are putting the production file inside the nginx/html folder, "EXPOSE 80" we are exposing the port 80 for outside checking the container



# DeployAngularAppGKE

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).






