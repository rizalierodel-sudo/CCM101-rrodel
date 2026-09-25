# Multi-Tier Architecture

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests from users. In this activity, the Nextcloud container works as the web/application tier.

## The Database Tier

The Database Tier is responsible for storing persistent data such as user accounts, file information, and other application data. In this activity, the MariaDB container works as the database tier.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage and maintain. It also keeps the application and database separated, so changes or problems in one container are less likely to affect the other.

