# Understanding Two-Tier Architecture

## The Web/Application Tier

The Web/Application Tier handles the user interface and processes requests from users. 
In this activity, Nextcloud serves as the web application and receives requests from the browser through the exposed port.

## The Database Tier

The Database Tier is responsible for storing the information needed by the application. 
In this activity, MariaDB stores the data used by Nextcloud, including user information and file metadata.

## Why Separate Them?

Separating the web application and database into two containers helps keep their functions organized. 
Each container has its own role, making the system easier to manage and allowing the application and database to be maintained separately.
