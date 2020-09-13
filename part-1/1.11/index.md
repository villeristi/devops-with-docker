```bash
➜  devops-with-docker/part-1 @ master ✗ touch /tmp/logs.txt && docker build . -t backend && docker run -d -p 8000:8000 -v /tmp/logs.txt:/usr/src/app/logs.txt backend
```
