# Microfrontend prototype for restaurant ordering.

## What is this?
This is an web project created with the library https://single-spa.js.org/.

It includes an prototype for an restaurant ordering application.

## Local development
    
1. **root-config**: Single-spa root, bootstrap and loads each SPA

    ```
    cd root-config
    npm install
    npm start
    ```

2. **Navbar**: Angular 12 navbar which is always displayed on screen

    ```
    cd navbar
    npm install
    npm start
    ```

3. **Discover**: Angular 12 application for displaying restaurants

    ```
    cd discover
    npm install
    npm start
    ```

4. **Order**: Angular 12 application for displaying and handling orders

    ```
    cd order
    npm install
    npm start
    ```

5. **Server**: dotnet 5 WebAPI with services for ordering and restaurants
    ```
    cd server
    docker-compose -f "docker-compose.yml" up -d --build
    ```

6. Navigate to http://localhost:9000 in a browser of your choice.
