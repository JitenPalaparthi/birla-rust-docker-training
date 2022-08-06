# Install

- On windoes you need to install putty tool.
- Step-1 : https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

## docker-commands

- ```docker info```
## Login

- Provide dockerhub username and password
    ```docker login``` 

- To pull docker image
    ```docker pull ubuntu```

    ```docker image inspect ubuntu```

    ```docker image history ubuntu```

- To delete an image
    ```docker rmi -f ubuntu``` or ```docker image rm ubuntu```


- To create a container and run
    ```docker run -it --name u1 ubuntu bash```
- To list running containers
    ```docker ps```
- To list all container
    ```docekr ps -a```
- start a stopped container
    ```docker start u1```
- exec into a running container
    ```docker exec -it u1 bash```
- To delete a container
    ```docker rm u1```
- To forcefully delete a container
    ```docker rm -f u1```
- To delete all containers
    ```docker rm -f $(docker ps -aq)```

- To get logs
    ```docker logs u1```
- To get follow logs
    ```docker logs -f u1```

- To build Dockerfile. The file name is Dockerfile
    ```docker build . -t jpalaparthi/ubuntuwithvim```

- To build docker with a different filename and a tag
    ```docker build -f DockerfileWithRust . -t jpalaparthi/ubuntuwithrust:0.0.1```

- To push images to docker

```docker push jpalaparthi/ubuntuwithrust:0.0.1```