## Scala barcelona Spark coding dodjo  Dockerfile

This repository contains a **Dockerfile** to create a docker container with Java 1.8, Maven 3 and git

### Dependencies

* [dockerfile/java](http://dockerfile.github.io/#/java)


### Installation

1. Install [Docker](https://www.docker.io/).

2. Clone the project

3. Build the image. The final dot is important, it's the path to **Dockerfile**. Replace **morfeo8marc** with your desired username (It takes a while):
`docker build -t morfeo8marc/scaladevbcn-spark-dojo .`


### Usage (two options)

#### 1. Run container and clone git repo into container

    docker run -i -t --name=spark-dojo <your_desired_username>/scaladevbcn-spark-dojo
    git clone <your repo url>
#### 2. Run container with git repo attached container (from host OS)

    docker run -i -t --name docker-java8-maven -rm -v <your git repo directory>:/volume/git <your_desired_username>/docker-java8-maven


I would like to thank [James D Bloom](http://blog.jamesdbloom.com) for his example container
