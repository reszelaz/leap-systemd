# leap-systemd
Docker image configuration for openSUSE Leap allowing to use systemd init scripts.

# How to start it?
Run it in detached mode and later on execute bash in order to play with it. Don't forget to mount the cgroup volume:

~~~~
docker run -d --name=leap -v /sys/fs/cgroup:/sys/fs/cgroup:ro reszelaz/leap-systemd;
docker exec -it leap bash
~~~~
