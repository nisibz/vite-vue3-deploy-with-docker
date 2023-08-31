# vite-vue3

This repository contains a Docker Compose configuration for deploying a Vite Vue3 application using Traefik as a reverse proxy with automatic HTTPS configuration. The setup allows you to quickly deploy your Vite Vue3 application with proper routing and secure HTTPS access.
## Before You Begin

If you don't have a Traefik network set up, you can follow the instructions in [this repository](https://github.com/nisibz/setup-traefik-with-docker.git) to create the necessary network configuration.

## Prerequisites

Before using this Docker Compose setup, make sure you have the following:

- Docker installed on your machine or server.
- A registered domain name for which you can configure DNS records.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/nisibz/vite-vue3-deploy-with-docker.git
   cd vite-vue3-deploy-with-docker
   ```

2. Update the `docker-compose.yml` file with your specific configurations:

   - Replace `your_domain` with your actual domain name in the `labels` section for both web and web-secure services.

3. Build and start the services using Docker Compose:

   ```bash
   docker-compose up -d
   ```