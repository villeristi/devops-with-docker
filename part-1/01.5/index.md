```bash
 ➜  devops-with-docker @ master ✗ docker run -d --name curl -it ubuntu:18.04 sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
Unable to find image 'ubuntu:18.04' locally
18.04: Pulling from library/ubuntu
f08d8e2a3ba1: Pull complete
3baa9cb2483b: Pull complete
94e5ff4c0b15: Pull complete
1860925334f9: Pull complete
Digest: sha256:05a58ded9a2c792598e8f4aa8ffe300318eac6f294bf4f49a7abae7544918592
Status: Downloaded newer image for ubuntu:18.04
7e634f7b0c6b54db49d76841e977a792e4a4a1d9b4154f20472d803e0fb69101

 ➜  devops-with-docker @ master ✗ docker exec curl sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
Input website:
Searching..
sh: 1: curl: not found

 ➜  devops-with-docker @ master ✗ docker exec curl sh -c 'apt-get update && apt-get install curl -y'
Hit:1 http://security.ubuntu.com/ubuntu bionic-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu bionic InRelease
Hit:3 http://archive.ubuntu.com/ubuntu bionic-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu bionic-backports InRelease
Reading package lists...
Reading package lists...
Building dependency tree...
Reading state information...
The following additional packages will be installed:
...

 ➜  devops-with-docker @ master ✗ docker attach curl
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```
