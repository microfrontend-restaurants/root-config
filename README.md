# Microfrontend prototype for restaurant ordering.

## What is this?
This is an web project created with the library https://single-spa.js.org/.
It includes an prototype for a restaurant ordering application.

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
