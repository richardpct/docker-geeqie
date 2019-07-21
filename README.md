# Purpose
Run Geeqie in a container

# Requirements
* MacOS
* Docker
* XQuartz

# Usage
I wrote a Makefile for handling the life cycles of images and containers, the
syntax is as follows:

## Building the image
    $ make build

## Running the container
    $ make run

By default the saved files are stored in ~/container/geeqie on your host, you
can change the directory by overriding the *VOL_SHARE* variable, for
instance:

    $ make VOL_SHARE=~/geeqie run

## Getting a shell access to the running container
    $ make exec

## Stopping the container
    $ make stop

## Removing the image
    $ make rm
