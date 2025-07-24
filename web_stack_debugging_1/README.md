# Nginx Port Configuration Script

This repository contains a Bash script to configure Nginx to listen on port 80 instead of the default port (8080). It automates the process of setting up Nginx by linking the default site configuration and ensuring that it is properly running.

## Script Overview

The main script is named `0-nginx_likes_port_80.sh`. It performs the following actions:

- Installs Nginx if it is not already installed.
- Removes any existing configurations in `sites-enabled`.
- Creates a symbolic link to the default site configuration in `sites-available`.
- Checks if Nginx is currently running on port 8080 and updates the configuration to listen on port 80.
- Starts the Nginx service.
- Allows traffic through the firewall on port 80.
- Reloads Nginx to apply the changes.
