# Search dockehub for neo4j
 docker search neo4j

#Pulling a docker image
docker pull neo4j

# Running a docker
docker run \                                        #base command
    --detach                                        # run docker in background
    --name  <name>                                  # container name
    --publish=7474:7474 --publish=7687:7687 \       # which port to use <choice>:<default>
    --volume=$HOME/neo4j/data:/data \               # where to store data
    neo4j                                           #what to run



# Stopping a running a container
docker stop <container name>


# removing a container
docker rm <container name>
