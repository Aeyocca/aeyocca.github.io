---
layout: post
title: Run PAUP with Docker
full-width: false
---

A pair of mutuals on Bluesky have recently claimed an error message running the latest version of PAUP on M1 chip Macs. Error messages akin to `error while loading shared libraries: libgfortran.so.4`

I've written a short [Dockerfile](https://aeyocca.github.io/assets/Dockerfile_paup) I got to work on my ARM64 Mac (at least got it to print the help message).

Put that buildfile in a directory with the [ubuntu binary](https://phylosolutions.com/paup-test/paup4a169_ubuntu64.gz) unzipped and changed permissions to 755 with 

`chmod 755 paup4a169_ubuntu64`

Then build with the following command or with you're own flavor of `docker build`

`docker buildx build --platform linux/amd64 --no-cache -t paup_test -f ./Dockerfile_paup .`

Took me about 10 minutes to build. Not sure if you've used docker much, but when running containers, you need to mount your current directory to the container to make your data available. Then you need to set the working directory inside container to where you mounted your data. I like using `/Z` because its short to write and unlikely to exist already.

eg. 
`docker run -v $PWD:/Z -w:/Z paup_test:latest paup4a169_ubuntu64`

Disclaimer: I'm a biologist first, and a poor programer second.
