# Microfrontend Prototype and examples

## What is this?
This is an demo micro front end web project created with https://single-spa.js.org/.
It includes examples for nginx and web components but also an prototype for a restaurant ordering application.

The prototype has an dotnet backend and a frontend with an app-shell and several different microfrontend components.

## Local development
    
1. **App-Shell**: Single-spa root, bootstrap and loads each SPA

    ```
    cd app-shell
    npm install
    npm start
    ```

2. **Navbar**: Angular 12 navbar which is always displayed on screen

    ```
    cd navbar
    npm install
    npm run serve:single-spa:navbar
    ```

3. **Discover**: Angular 12 application for displaying restaurants

    ```
    cd discover
    npm install
    npm run serve:single-spa:discover
    ```

4. **Order**: Angular 12 application for displaying and handling orders

    ```
    cd order
    npm install
    npm run serve:single-spa:order
    ```

5. **Server**: dotnet 5 WebAPI with services for ordering and restaurants
    ```
    cd server
    docker-compose -f "docker-compose.yml" up -d --build
    ```