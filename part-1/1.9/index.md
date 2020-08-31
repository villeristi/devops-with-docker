```bash
 ➜  devops-with-docker/part-1 @ master ✗ docker run -p 80:80 --rm devopsdockeruh/ports_exercise
Unable to find image 'devopsdockeruh/ports_exercise:latest' locally
latest: Pulling from devopsdockeruh/ports_exercise
cbdbe7a5bc2a: Already exists
fb0e3739aee1: Pull complete
738de7869598: Pull complete
ffd68be3d86c: Pull complete
d6a92ac5065d: Pull complete
8deb0960be38: Pull complete
aec7a3bd83e0: Pull complete
8f73392c117e: Pull complete
Digest: sha256:9779e303353ef47da9ea0223bfbb9fbdb8f8fe39178e2e06153027e28e9e5400
Status: Downloaded newer image for devopsdockeruh/ports_exercise:latest

> ports_exercise@1.0.0 start /usr/app
> node index.js

Listening on port 80, this means inside of the container. Use -p to map the port to a port of your local machine.
```
