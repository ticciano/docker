<h1 align="center"> Backup and restore containers </h1>

Backup

Make desired changes to container

Commit changes
docker commit containername containername:tag

Use docker save to export image
docker image save image:tag > image-version.img

Restore

Import image in destination 
docker load -i image-version.img> :construction: Projeto em construção :construction: