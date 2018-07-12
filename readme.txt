# Search dockehub for neo4j
 docker search neo4j

#Pulling a docker image
docker pull neo4j

# Running a neo4J docker
docker run \                                        #base command
    --detach                                        # run docker in background
    --name  <container_name>                                  # container name
    --publish=7474:7474 --publish=7687:7687 \       # which port to use <choice>:<default>
    --volume=$HOME/neo4j/data:/data \               # where to store data
    neo4j                                           #what to run



# Stopping a running a container
docker stop <container_name>


# removing a container
docker rm <container_name>


# Entering inside a running container
docker exec -it <container_name> bash


# Running a mysql container on port 7487
docker run --name Ranu_mysql -e MYSQL_ROOT_PASSWORD=root  --publish=7487:3306  -d mysql:5.7
