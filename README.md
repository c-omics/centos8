# BioInformatics Docker Images

## Useful Links:
 * [github-site](https://github.com/c-omics) for source
 * [Docker Hub](https://hub.docker.com/u/comics) for docker images

## Dockerfiles
 1. The respective license of the applications is located at /usr/share/licenses/ within the docker image. 
 2. Most ```comics``` dockerfiles inherit the base ```comics/centos8``` image, which in turn is based on the official centos:8 image.
 3. At build-time, the images will download and install 3rd party software. While we try to verify the authenticity of such software, this is not easily achieved, particularly when the 3rd party software itself pulls in dependencies.
 4. Many images will install software from source. To keep the images light-weight, where possible the dockerfile will download the software, verify it, build it, and remove the source again within a single RUN instruction. 
 

