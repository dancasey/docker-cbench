# docker-cbench

[cbench](https://github.com/andi-bigswitch/oflops/tree/master/cbench) on [Docker](https://www.docker.com), via [mininet](http://mininet.org).


## Get

`docker pull dancasey/docker-cbench`


## Use

Uses `ENTRYPOINT` so that the container can be run with arguments to override `CMD`, e.g.,

    docker run -it --rm --link ryu dancasey/cbench -c ryu -p 6653 -s 2

The default `CMD` tries to connect to `controller` at port `6653` with cbench's defaults (16 switches, 16 loops, etc.).


## License

This tiny Dockerfile is released under [PDDL-1.0](https://spdx.org/licenses/PDDL-1.0). You probably want to check the licenses of [cbench (from oflops)](https://github.com/andi-bigswitch/oflops/blob/master/COPYING) and [mininet](https://github.com/mininet/mininet/blob/master/LICENSE).
