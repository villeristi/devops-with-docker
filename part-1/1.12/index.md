```bash
 ➜  devops-with-docker/part-1 @ master ✗ docker build -f Dockerfile.front -t frontend . && docker build -f Dockerfile.back -t backend .
 ➜  devops-with-docker/part-1 @ master ✗ docker run -d -p 5000:5000 frontend && docker run -d -p 8000:8000 -v /tmp/logs.txt:/usr/src/app/logs.txt backend
```
