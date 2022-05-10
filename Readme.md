# Cara Simple Upgrade Laravel 8 ke Laravel 9

## Updating Dependencies
1. Laravel 9 membutuhkan PHP versi 8.0.2 atau lebih.
2. Update Composer dependecies pada file ```composer.json``` yaitu pada:
    ```sh
    laravel/framework to ^9.0
    nunomaduro/collision to ^6.1

    ```
    dan
    ```facade/ignition``` with ```"spatie/laravel-ignition": "^1.0"``` pada file ```composer.json```.    

3. run ```composer update``` pada folder project.
4. Jika terdapat error pada file dependecies lain, maka cek dokumetasi file dependecies (cek web resmi / github).
   seperti contoh:
   ```sh
        Your requirements could not be resolved to an installable set of packages.

        Problem 1
            - realrashid/sweet-alert v4.0.0 requires laravel/framework ^7.0|^8.0 -> found laravel/framework[v7.0.0, ..., 7.x-dev, v8.0.0, ..., 8.x-dev] but it conflicts with your root composer.json require (^9.0).
            - realrashid/sweet-alert v4.1.0 requires laravel/framework ^5.6|^6.0|^7.0|^8.0 -> found laravel/framework[v5.6.0, ..., 5.8.x-dev, v6.0.0, ..., 6.x-dev, v7.0.0, ..., 7.x-dev, v8.0.0, ..., 8.x-dev] but it conflicts with your root composer.json require (^9.0).
            - Root composer.json requires realrashid/sweet-alert ^4.0 -> satisfiable by realrashid/sweet-alert[v4.0.0, v4.1.0].
    ```

    maka silahkan cek ke website dokumetasi dari ```realrashid/sweet-alert``` (https://github.com/realrashid/sweet-alert/releases).

