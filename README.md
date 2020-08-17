# Static File Server

This repository contains nginx configuration that is optimized for serving static files.

## Requirements

This configuration is optimized for:

1. A container/VM/dedicated server that is behind a load balancer (proxy protocol is required).
2. SSL is handled by another web server.
3. A web application that only contains static files (e.g. html, css, js, and etc) that can be a SPA (fallback is handled).

## Installation

### Step 1

Copy your entire app (everything that should be served on the web including css, js, and etc) in to `app/wwwroot`.

### Step 2

To use this configuration, please mount the folders below:

1. `app` to `/app`.
2. `/etc/nginx` to `/etc/nginx`.
