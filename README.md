DockerNexpose
=============
[![](https://badge.imagelayers.io/whithajess/dockernexpose:latest.svg)](https://imagelayers.io/?images=whithajess/dockernexpose:latest 'Get your own badge on imagelayers.io')

Uses the nexpose chef cookbook to create a nexpose docker container

USAGE
=============

### Pull Down Image
```bash
docker pull dprauser/InsightVM-Console-Docker
```

### Deamonize Image
```bash
sudo docker run \
  --name rapid7-insightvm-console \
  -p 3780:3780 \
  -d dprauser/InsightVM-Console-Docker
```

### Check State
Nexpose takes awhile to set up all its stuff.
`docker attach $PID` should show you where its up to.

### Log In
  * use your local browser port 49160: https://localhost:49160/
  * default username/password is nxadmin/nxadmin
  * will need to active community license here etc.
