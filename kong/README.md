<!--

********************************************************************************

WARNING:

    DO NOT EDIT "kong/README.md"

    IT IS AUTO-GENERATED

    (from the other files in "kong/" combined with a set of templates)

********************************************************************************

-->

# Quick reference

-	**Maintained by**:  
	[the Kong Docker Maintainers](https://github.com/kong/kong)

-	**Where to get help**:  
	[the Docker Community Slack](https://dockr.ly/comm-slack), [Server Fault](https://serverfault.com/help/on-topic), [Unix & Linux](https://unix.stackexchange.com/help/on-topic), or [Stack Overflow](https://stackoverflow.com/help/on-topic)

# Supported tags and respective `Dockerfile` links

-	[`3.5.0-ubuntu`, `3.5-ubuntu`, `3.5.0`, `3.5`, `3`, `latest`, `ubuntu`](https://github.com/Kong/docker-kong/blob/e4ba2e351f3da34727fd016409a2669004b3fce0/ubuntu/Dockerfile)
-	[`3.4.2-ubuntu`, `3.4-ubuntu`, `3.4.2`, `3.4`](https://github.com/Kong/docker-kong/blob/2ccc1a4cc237f2cbe85e9226c8d0fa1e70f1d612/ubuntu/Dockerfile)
-	[`3.3.1-alpine`, `alpine`](https://github.com/Kong/docker-kong/blob/2207aa20530f8a04290c82c9c2258717f7795080/Dockerfile.apk)
-	[`3.3.1-ubuntu`, `3.3-ubuntu`, `3.3.1`, `3.3`](https://github.com/Kong/docker-kong/blob/2207aa20530f8a04290c82c9c2258717f7795080/ubuntu/Dockerfile)
-	[`3.2.2-alpine`](https://github.com/Kong/docker-kong/blob/5641f8836920650fc66c6d36408daf794d730b96/Dockerfile.apk)
-	[`3.2.2-ubuntu`, `3.2-ubuntu`, `3.2.2`, `3.2`](https://github.com/Kong/docker-kong/blob/5641f8836920650fc66c6d36408daf794d730b96/ubuntu/Dockerfile)
-	[`3.1.1-alpine`, `3.1.1`, `3.1`](https://github.com/Kong/docker-kong/blob/5f914be945ec1732837cc4f6463219bed566c7ef/Dockerfile.apk)
-	[`3.1.1-ubuntu`, `3.1-ubuntu`](https://github.com/Kong/docker-kong/blob/5f914be945ec1732837cc4f6463219bed566c7ef/ubuntu/Dockerfile)
-	[`2.8.4-alpine`, `2.8.4`, `2.8`](https://github.com/Kong/docker-kong/blob/1c31704cdc9bbd2c0a20e5479eb307140339582b/alpine/Dockerfile)
-	[`2.8.4-ubuntu`, `2.8-ubuntu`](https://github.com/Kong/docker-kong/blob/1c31704cdc9bbd2c0a20e5479eb307140339582b/ubuntu/Dockerfile)

# Quick reference (cont.)

-	**Where to file issues**:  
	[https://github.com/kong/kong/issues](https://github.com/kong/kong/issues?q=)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/kong/), [`arm64v8`](https://hub.docker.com/r/arm64v8/kong/)

-	**Published image artifact details**:  
	[repo-info repo's `repos/kong/` directory](https://github.com/docker-library/repo-info/blob/master/repos/kong) ([history](https://github.com/docker-library/repo-info/commits/master/repos/kong))  
	(image metadata, transfer size, etc)

-	**Image updates**:  
	[official-images repo's `library/kong` label](https://github.com/docker-library/official-images/issues?q=label%3Alibrary%2Fkong)  
	[official-images repo's `library/kong` file](https://github.com/docker-library/official-images/blob/master/library/kong) ([history](https://github.com/docker-library/official-images/commits/master/library/kong))

-	**Source of this description**:  
	[docs repo's `kong/` directory](https://github.com/docker-library/docs/tree/master/kong) ([history](https://github.com/docker-library/docs/commits/master/kong))

# What is Kong?

Kong Gateway is the world’s most adopted API gateway. Lightweight, fast, and flexible, this open source gateway is built for hybrid and multi-cloud and optimized for microservices and distributed architectures.

Built on this open source DNA, Kong’s unified cloud API platform helps organizations ranging from startups to Fortune 500 enterprises unleash developer productivity, build securely, and accelerate time to market.

Kong's official documentation can be found at [docs.konghq.com](https://docs.konghq.com/).

# How to use this image

Please refer to the [installation section](https://docs.konghq.com/gateway/latest/install/docker/#main) on our documentation website to learn how to use this image.

# Image Variants

The `kong` images come in many flavors, each designed for a specific use case.

## `kong:<version>`

This is the defacto image. If you are unsure about what your needs are, you probably want to use this one. It is designed to be used both as a throw away container (mount your source code and start the container to start your app), as well as the base to build other images off of.

## `kong:<version>-alpine`

This image is based on the popular [Alpine Linux project](https://alpinelinux.org), available in [the `alpine` official image](https://hub.docker.com/_/alpine). Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

This variant is useful when final image size being as small as possible is your primary concern. The main caveat to note is that it does use [musl libc](https://musl.libc.org) instead of [glibc and friends](https://www.etalabs.net/compare_libcs.html), so software will often run into issues depending on the depth of their libc requirements/assumptions. See [this Hacker News comment thread](https://news.ycombinator.com/item?id=10782897) for more discussion of the issues that might arise and some pro/con comparisons of using Alpine-based images.

To minimize image size, it's uncommon for additional related tools (such as `git` or `bash`) to be included in Alpine-based images. Using this image as a base, add the things you need in your own Dockerfile (see the [`alpine` image description](https://hub.docker.com/_/alpine/) for examples of how to install packages if you are unfamiliar).

# License

View [license information](https://konghq.com/kong/license/) for the software contained in this image.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

Some additional license information which was able to be auto-detected might be found in [the `repo-info` repository's `kong/` directory](https://github.com/docker-library/repo-info/tree/master/repos/kong).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
