# Distroless Docker Image Example

This repository provides an example of a Distroless Docker image running a basic Express server. 

The name "distroless" is catchy. In reality, there is no such a thing as a distroless docker image. The image still need a user space but in this case, we are using someone else (Google)'s distro. What we then get is a slimmed down environment without package managers, shells or other apps you might find in a typical distribution. 

## Prerequisites
Before running the application, ensure that you have [Docker](https://docs.docker.com/get-docker/) installed on your system.

## Usage

1. Clone this repository to your local machine and change to the cloned directory:

    ```
    git clone https://github.com/kabandr/distroless.git
    cd distroless
    ```

2. Build the Docker image using the provided Dockerfile:

    ```
    docker build -t distroless .
    ```

3. Run the container:
    ```
    docker run -p 3000:3000 distroless
    ````
    This command maps port 3000 of the container to port 3000 of the host system. Adjust the port mapping as per your requirement.

## License
This example is provided under the MIT License. Feel free to use and modify it according to your needs.

## Acknowledgments

Special thanks to the open-source community.

If you have any questions or feedback, please don't hesitate to reach out.