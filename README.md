<header>

# Publish to GitHub Packages

_Use GitHub Actions to publish your project to a Docker image._

</header>

## Step 2: Add a Dockerfile

_You created a publishing workflow! :tada:_

We will add a `Dockerfile` to the `cd` branch. The `Dockerfile` contains a set of instructions that get stored in a `Docker Image`. If you'd like, you can [learn more about Dockerfiles](https://docs.docker.com/engine/reference/builder/).

### :keyboard: Activity: Add a Dockerfile

1. In the `cd` branch, create `Dockerfile` at the project root and include:
   ```dockerfile
   FROM nginx:1.24-alpine
   COPY . /usr/share/nginx/html