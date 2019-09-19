# The Alpine Docker image with latest GCC

This image is based on Alpine Linux image and contains [C/C++ compiler](https://gcc.gnu.org/) (GCC 7/8/9).

## Docker Hub images

```
$ docker pull n0madic/alpine-gcc:7.4.0
or
$ docker pull n0madic/alpine-gcc:8.3.0
or
$ docker pull n0madic/alpine-gcc:9.1.0
```

## Build image and usage

```
$ git clone https://github.com/n0madic/alpine-gcc.git
$ cd alpine-gcc
$ docker build --build-arg GCC_VERSION=7.4.0 --build-arg ALPINE_VERSION=3.10 -t alpine-gcc .
or
$ docker build --build-arg GCC_VERSION=8.3.0 --build-arg ALPINE_VERSION=3.10 -t alpine-gcc .
$ docker run --rm -it -v $(pwd):/src alpine-gcc
```
