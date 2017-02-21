# base

A minimal Alpine-based docker image which includes:

* openssl
* ca-certificates
* [dumb-init](https://github.com/Yelp/dumb-init), which makes it easy to configure child process reaping and gives us signal forwarding to all processes running under it
* [su-exec](https://github.com/ncopa/su-exec), which makes it less of a pain to switch to other users without introducing a `su` or `sudo` intermediate process


Use it in a Dockerfile:
   
```
FROM lewispeckover/base
```
Find it on [Docker Hub](https://hub.docker.com/r/lewispeckover/base/).
