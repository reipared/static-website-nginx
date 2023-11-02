# Static Website with Nginx and Docker

This repository demonstrates how to containerize and serve a static website using Nginx and Docker. It's a straightforward setup that allows you to quickly get your website up and running.

## Steps to Deploy Your Website

### 1. Create Your Website Files

Create the website files, including `index.html`, `style.css`, `script.js`, and any other assets you need.

### 2. Create a Dockerfile

Create a `Dockerfile` in your project directory.

### 3. Build the Docker Image

Assuming you have Docker installed and running, build the Docker image by running the following command in your project directory:

`docker build -t webserver-image:v1 .`

### 4. Run the Docker Container

Start a Docker container using the built image:

`docker run -d -p 80:80 webserver-image:v1`

### 5. Access your website

Visit `http://localhost:80` in your web browser to view your static website.

## Customizing Nginx configuration

If you need to customize the Nginx configuration for your website, you can modify the `nginx.conf` file in your project directory. After making changes, rebuild the Docker image and restart the container.

## Next Steps

If you plan to deploy your website to a production server, consider pushing your Docker image to a container registry and setting up a more robust production environment.

That's it!
