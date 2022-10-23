<h1 align="center"> Backup and restore containers </h1>

> <h2>Backup</h2>

After making desired changes to container, do the following assuming container name *api-gateway*

Commit changes
```
docker commit api-gateway api-gateway:1.0
```

Use docker save to export image
```
docker image save api-gateway:1.0 > api-gateway_1.0.img
```

[!NOTE]
The file extensions is not relevant.


> <h2>Restore</h2>

1. Import image in destination

```
docker load -i api-gateway_1.0.img>
```

2. Run a new container

```
docker run -d api-gateway:1.0
```

