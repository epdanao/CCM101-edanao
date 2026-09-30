# Understanding Two-Tier Architecture

## The Web/Application Tier

The Web/Application Tier is responsible for providing the user interface and handling requests from users. 
In this activity, the Nextcloud application acts as the web tier and receives browser requests through the exposed port.

## The Database Tier

The Database Tier stores persistent information needed by the application. 
In this activity, MariaDB stores the database information used by Nextcloud, including data related to users and file metadata.

## Why Separate Them?

Separating the web application and database into two containers keeps their responsibilities organized. 
Each container can focus on its own role, which makes the system easier to manage and allows the application and database to be handled separately.
