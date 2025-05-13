# funydockerfile
A loser minimal Docker image that serves a static website using Nginx. Automatically downloads HTML from my gitHub repo during build. It's not even useful. Just funny.
IF YOU DONT KNOW HOW TO INSTALL DOCKER AND WHAT DOCKER IS : https://docs.docker.com/engine/install/centos/

## How to install:

1. **pull the dockerfile:**
   first clone the repository:
```
   git clone https://github.com/plocord/funydockerfile
```


2. **Build the image:**
Navigate to the directory containing the dockerfile then run:
```
   docker build -t funnyserver .
```

This command builds the loser docker image named `funnyserver` using the Dockerfile and HTML files in the current directory.

3. **Run the Container:**
After building the image, you can run the slave(container) with a port:
```
   docker run -d -p 8080:80 funnyserver
```

This command runs the container in detached mode (`-d`) and maps port 8080 on the host to port 80 in the container.

4. **Try it Out:**
Open ur favorite web browser and navigate to `http://localhost:8080`. If u did everything right u should see the website on screen

5. **Stop the Container:**
If you're done playing around, you can stop the container by running:
```
   docker stop <container_id>
```

Replace `<container_id>` with the ID of the running container.

That's it.

btw u can js replace the source website by replacing the link on line 4
~


