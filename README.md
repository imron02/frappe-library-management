## Library Management

Library Management System

## Installation

> **Note:** This app is only compatible with Frappe v14.x.x.

## Rule

- The Frappe framework uses `_` instead of `-` for the app name. For example, `library-management` becomes `library_management`.

1. Install [bench & frappe](https://frappeframework.com/docs/v14/user/en/installation). or run the following command

   ```
   $ bench init library-bench --version version-14 && cd library-bench
   ```

2. After successfully, please install the **library_management** app by running
   ```
   $ bench get-app library_management https://github.com/imron02/frappe-library-management.git
   ```

4. After successfully installing the app, you need create example site by running
   ```
   $ bench new-site library.test
   $ bench use library.test
   ```

4. Install the app on the required site by running
   ```
   $ bench --site library.test install-app library_management
   ```

5. Migrate the database by running
   ```
   $ bench start
   $ bench migrate
   ```

#### License

MIT