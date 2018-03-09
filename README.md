# docker-openrefine
Docker recipes for OpenRefine

## To Build

```
docker build -t="eo4/openrefine:2.8" https://github.com/EO4/docker-openrefine.git#master:alpine-jre8-openrefine
```

## To Run

-p option port localhost:3333 to container; goto localhost:3333 to see OpenRefine.

-v option links a volume, replace [DIR] with path to the data directory you wish to link

Not sure if this is necessary, maybe to save templates?

For example:
~/Documents/eo4/my-cool-project:/data


```
docker run -p "3333:3333" openrefine:2.8
```

Don't forget to stop the container!

```
docker ps
docker stop [CONTAINER ID]
```

