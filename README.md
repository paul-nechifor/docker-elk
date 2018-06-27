# This repository has been moved to [gitlab.com/paul-nechifor/docker-elk](http://gitlab.com/paul-nechifor/docker-elk).

Old readme:

# Docker ELK stack (Python example)

This is a fork of [Docker ELK stack][original] to which I added a small Django
service for testing purposes.

## Usage

[Read the full instructions from fork source][original].

Run this fix:

    sudo sysctl -w vm.max_map_count=262144

Get it up:

    docker-compose up

Services:

* [Kibana is at localhost:5601](http://localhost:5601/).
* [The Django service is at localhost:3000](http://localhost:3000/).

Currently the service doesn't do anything, it just errors with `ImportError: No
module named urls` which gets logged into the ELK stack.

## License

MIT

[original]: https://github.com/deviantony/docker-elk
