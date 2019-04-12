# ps2dev-docker

![BSD-2 License](https://img.shields.io/badge/license-BSD--2-blue.svg)
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/root670/ps2dev-docker.svg)
![Docker Pulls](https://img.shields.io/docker/pulls/root670/ps2dev-docker.svg)

A Docker image for building PlayStation 2 homebrew applications using PS2SDK.
Based on [ps2dev/ps2dev-docker](https://github.com/ps2dev/ps2dev-docker) with
changes to support building my projects.

## Original readme.txt
```
 ====================
  What does this do?
 ====================

  This program will automatically build a docker image with the ps2dev
  toolchain ready to be used for homebrew development.

 ====================
  How do I build it?
 ====================

 Build the image:

   docker build -t ps2dev-docker .

 Copy the helper script:

   cp ps2dev-docker.sh /usr/local/bin

 ==================
  How do I use it?
 ==================

 Use the helper script to run 'make' on the current directory:

   ps2dev-docker.sh make

 ============================
  How do I save and load it?
 ============================

 Save the image:

   docker save ps2dev-docker | bzip2 > ps2dev-docker.tar.bz2

 Load the image:

   docker load < bzip2 -dc ps2dev-docker.tar.bz2
```