# Substrate Telemetry Backend DAppNode Package

Dappnode package [metadata wrapper](dappnode_package.json) and [docker image](./build/Dockerfile) based on [Substrate-telemetry from Parity Tech](https://github.com/paritytech/substrate-telemetry.git) 

- This is the [DAppNode Package Substrate Telemetry Backend](https://github.com/luguslabs/DAppNodePackage-substrate-telemetry-backend/releases) running backend part only.
If you want to run both frontend and backend or just Telemetry frontend install this [DAppNode Package Substrate Telemetry](https://github.com/luguslabs/DAppNodePackage-substrate-telemetry) instead.

- Frontend Telemetry Package can connect to this standalone Telemetry backend Package be configuring `REMOTE_PUBLIC_IP_TELEMETRY_BACKEND` in frontend package env.

- [Install latest release here](https://github.com/luguslabs/DAppNodePackage-substrate-telemetry-backend/releases) of this DAppNode Package. 

It is an AragonApp whose repo is deployed at this address: [0x9f85ae5aefe4a3eff39d9a44212aae21dd15079a ](https://etherscan.io/address/0x9f85ae5aefe4a3eff39d9a44212aae21dd15079a) and whose ENS address is: [substrate-telemetry-backend-archipel.public.dappnode.eth](https://etherscan.io/enslookup?q=substrate-telemetry-backend-archipel.public.dappnode.eth])

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- git

  Install [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) commandline tool.

- docker

  Install [docker](https://docs.docker.com/engine/installation). The community edition (docker-ce) will work. In Linux make sure you grant permissions to the current user to use docker by adding current user to docker group, `sudo usermod -aG docker $USER`. Once you update the users group, exit from the current terminal and open a new one to make effect.

- docker-compose

  Install [docker-compose](https://docs.docker.com/compose/install)

**Note**: Make sure you can run `git`, `docker ps`, `docker-compose` without any issue and without sudo command.

###  No env parameters needed

## Running

### Start

```
$ docker-compose up -d
```

### Stop

```
$ docker-compose down
```

### Status

```
$ docker-compose ps
```

### Logs

```
$ docker-compose logs -f
```

## Contributing

Please read [CONTRIBUTING.md](TBD) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/luguslabs/DAppNodePackage-substrate-telemetry-backend/releases).

## Authors

- **Vladimir Ostapenco** - _Initial work_ - [vladostp](https://github.com/vladostp)
- **Francois Branciard** - _Initial work_ - [branciard](https://github.com/branciard)

See also the list of [contributors](https://github.com/luguslabs/DAppNodePackage-substrate-telemetry-backend/contributors) who participated in this project.

## License

This project is licensed under GPL3 - see the [LICENSE](LICENSE) file for details

## References

[git](https://git-scm.com/)

[docker](https://www.docker.com/)

[docker-compose](https://docs.docker.com/compose/)

[DappNode](https://www.dappnode.io/)


