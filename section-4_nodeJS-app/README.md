# Section 4: Simple NodeJS app
## Port forwarding
Starting a container  with the image does not  expose the containers port to the localhost network. In order to map the localhost port to the containers internal network, the ports need to be mapped in the `run` command.

Run the built image with the following command:
```shell
> docker run -p [localhost-port]:8080 [image-name]
```
