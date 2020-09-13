 ➜  devops-with-docker/part-1/1.7 @ master ✗ docker build -t curler . && docker run -ti curler
Sending build context to Docker daemon  3.072kB
Step 1/6 : FROM ubuntu:16.04
 ---> 4b22027ede29
Step 2/6 : RUN apt-get update && apt-get install -y curl
 ---> Using cache
 ---> cab59a1707c0
Step 3/6 : WORKDIR /app
 ---> Using cache
 ---> 930cbab9e176
Step 4/6 : COPY curler.sh .
 ---> 6d00f4c59a5f
Step 5/6 : RUN chmod +x curler.sh
 ---> Running in b39f52d43046
Removing intermediate container b39f52d43046
 ---> a63b3249405f
Step 6/6 : CMD ["./curler.sh"]
 ---> Running in 1232508d4c20
Removing intermediate container 1232508d4c20
 ---> 02f571083738
Successfully built 02f571083738
Successfully tagged curler:latest
Input website:
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
