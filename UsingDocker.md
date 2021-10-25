# Using Docker Images

* Using docker image: seurat
  * Once we have the image pulled, we need to follow this page to setup docker, so that we do NOT need to run it under root. sudo usermod -aG docker USERNAME
  * To all docker image to use local file system, we can do docker run -v /host/directory:/container/directory --it --rm imagename
  * To enable X11, we can do docker run -v /tmp/.X11-unix:/tmp/.X11-unix:rw -v /host/directory:/container/directory -e DISPLAY=$DISPLAY -it --rm imagename