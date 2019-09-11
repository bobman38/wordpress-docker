# Wordpress docker local setup

Very easy and simple docker local setup.

# How to use it ?

## Drop the code

Drop a working `wordpress` codebase inside the `wordpress` folder. It can be an existing code base with all plugins and content, or a newly wordpress install just downloaded  from https://wordpress.org.

You must have `wp-admin`, `wp-content` folders under `wordpress` (no additionnal subfolder)

##  Provide a existing database (optional)

If like me you want to duplicate an existing WP installation, you must provide also an export of the existing WP database. Drop the exported file as a replacement of `wordpress.sql` file. It will be loaded directly by the mariadb container at docker startup.

## Run docker

Start the stack with:

```
docker-compose up
```

Check on `http://localhost:8000`

Remove the stack by:

```
docker-compose down
```

Happy coding on wordpress :)
