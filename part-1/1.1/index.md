```bash
 ➜  devops-with-docker @ master ✓ docker ps -a
CONTAINER ID        IMAGE                                                 COMMAND                  CREATED             STATUS                   PORTS                    NAMES
5c830ad04520        docker.elastic.co/elasticsearch/elasticsearch:7.4.2   "/usr/local/bin/dock…"   3 days ago          Exited (1) 3 days ago                             smplf_portal_elasticsearch
38a31f5a23aa        redis:alpine                                          "docker-entrypoint.s…"   3 days ago          Up 3 days                0.0.0.0:6379->6379/tcp   smplf_portal_redis
b159bfff3735        postgres:11                                           "docker-entrypoint.s…"   11 days ago         Up 3 days                0.0.0.0:5434->5432/tcp   smplf_portal_db
9608c0cd7700        postgres:11                                           "docker-entrypoint.s…"   11 days ago         Exited (0) 11 days ago                            shoppie_db
```
