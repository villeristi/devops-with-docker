```bash
 ➜  devops-with-docker @ master ✗ docker run -d --name clock devopsdockeruh/exec_bash_exercise
73d1b699bab60279fd5ba2f2703b8861516e19a9c1c2393ae15e0714422d39a8
 ➜  devops-with-docker @ master ✗ docker exec clock tail ./logs.txt
Mon, 31 Aug 2020 18:35:05 GMT
Mon, 31 Aug 2020 18:35:08 GMT
Mon, 31 Aug 2020 18:35:11 GMT
Mon, 31 Aug 2020 18:35:14 GMT
Secret message is:
"Docker is easy"
```
