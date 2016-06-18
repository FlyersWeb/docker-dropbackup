# Dropbox synchronize backup

Sync dropbox folder without installing anything besides docker

## Install docker

See https://www.docker.com/ for more help

## How to build it

```
$ git clone https://github.com/FlyersWeb/docker-dropbackup.git
$ cd docker-dropbackup
$ docker build -t "dropbackup" .
```

## How to use

```
$ docker run -it -v /test/:/data -e TOKEN=xxxxxxxxxxxxxxxxxxxxxxx -e DEST=test -e PYTHONIOENCODING=utf8 dropbackup
```

## How it works

The image will synchronize ```/test/``` folder with the ```test``` dropbox folder provided by the DEST environment variable. You'll need an application token to use the dropbox API and provide it using the TOKEN environment variable.

## Conclusion

Feel free to use it but remember that This software is supplied "AS IS" without any warranties and support.

@flyersweb
