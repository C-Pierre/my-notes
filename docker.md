# <span style="color:#57B8FF; font-weight: bold">Docker</span>

## Remember me

        IMAGE: a compiled application   
        CONTAINER: a launched application   
        VOLUME: a folder shared by container and host, which can contain multiple containers

---

## Usefull commands

- ### List

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker images</span>  
to some *blue* text list all the local images

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker ps</span>     
to list all the running containers

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker ps --all</span>       
to list all the running containers (inclundind stopped once)

-----------

</div>

- ### Run / stop

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker run image-name</span>         
to create a container based on an image

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker run --env MYSQL_ROOT_PASSWORD=my-secret-pw image-name</span>          
to create a container setted with a mandatory environment variable

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker stop container-name</span>    
to stop the container (we can use the container id as well)

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker restart container-name</span>    
to restart the container (we can use the container id as well)

-----------

</div>

- ### Acces / debug

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker exec -it container-name bash</span>     
to acces to the running container (-i and -t options are used to access the container in an interactive mode and the bash command is used to get a bash shell inside the container.)

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker logs container-name</span>    
to help debgugging container (it will fetch logs from a specified container)

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker logs -follow container-name</span>    
to help debgugging container (and continue to streamup new output)

-----------

</div>

- ### Remove

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker rm container-name</span>      
to remove a container

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker rm -f container-name</span>   
to force to remove a container

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker rmi image-id</span>   
to remove an image

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker image prune</span>    
to clean up unused images

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker volume prune</span>   
to clean up unused volumes

<span style="color:#57B8FF; font-style: italic; font-weight: bold">docker container prune</span>        
to clean up unused volumes

-----------

</div>