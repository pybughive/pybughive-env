# PyBugHive Docker Environment

This repository contains the Docker environment for PyBugHive, with everything pre-installed.
We provide two Docker images: (1) the primary environment to use PyBugHive and (2) a customized MongoDB image that provides the database server.

## Usage

First, you need to clone this repository.
The building process will check out the main repository of PyBugHive, so if you use PyBugHive from Docker, you only need this repository.

```
git clone https://github.com/pybughive/pybughive-env.git
```

Navigate to the directory.

```
cd pybughive-env
```

Start the containers by using the *docker-compose* command.

```
docker-compose up -d
```

If you wish to modify the Docker files to install any convenience package, you may use `docker-compose up --build -d` to rebuild the images.
After the containers are up and running, you can connect to the *pybughive-env* container and start using PyBugHive.

```
docker exec -it pybughive-env /bin/bash
```
