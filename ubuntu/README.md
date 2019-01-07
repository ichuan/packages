# Ubuntu deb packages

## Packaging environment setup

Via [ostechnix](https://www.ostechnix.com/create-deb-file-source-ubuntu-16-04/)

```bash
sudo apt-get update
sudo apt-get -y install checkinstall build-essential automake autoconf \
  libtool pkg-config libcurl4-openssl-dev intltool libxml2-dev \
  libgtk2.0-dev libnotify-dev libglib2.0-dev libevent-dev wget

# TODO package configure and make

# make deb
sudo checkinstall
```

You can using docker to make packages for different dist:

```bash
docker run --rm -it -v `pwd`:/data ubuntu:18.04
```


## deb files
- install with `dpkg -i xx.deb`
- uninstall with `dpkg -r xx.deb`
