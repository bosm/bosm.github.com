---
layout: page
title: bosm
tagline: build your linux distribution from scratch made simple
---
{% include JB/setup %}

## why bosm

Building linux distribution from scratch may be hard, but should be simple --- in no more than two steps,

    fetch code ---> bosm

and, your distribution is ready to be consumed.

Reproducing a distribution from source the simple way may be good enough to make distribution user happy. However, what developer needs, out of a build system, is way more than that, to just list a few of them,

    - distribution should be customizable (true to user as well)
    - build fast and build in parallel
    - incremental build and per-package amend and rebuild
    - simple and clean way of install/uninstall package
    - in-place source code change with version control system
    - built-in cross compile support

bosm (b-awe-some) is designed to achieve all of the above and more.

## what bosm is and is not

bosm is a build system, bosm is not a linux distribution, it builds one (and more) of them. bosm is light weight and simple to use, and bosm has both user and developer support in mind.

bosm is a build system designed to help build your linux distribution and/or software with the following goals,

    - simple and easy to use
    - fast and incremental/parallel build
    - cross compile friendly
    - in-place source code change --- no build time copy/staging
    - open source licenses management
    - git integration

## test run

Sounds interesting? to try it out,

    repo init -u git://github.com/bosm/manifest && repo sync
    export PATH=$PWD/bos/bin:$PATH
    bosm
