Docker Commands

- DOCKER_OPTS="-H unix:///var/run/docker.sock -H tcp://0.0.0.0:2375"
- DOCKER_OPTS to modify the daemon startup options.  /etc/default/docker curl http://127.0.0.1:2375/info connection refused
- curl http://127.0.0.1:2375/info
- netstat -nlp|grep 2375
- Then run the daemon with the following command:
- service docker stop
- service docker stop
- nohup docker daemon -H tcp://0.0.0.0:2375 -H unix:///var/run/docker.sock &
