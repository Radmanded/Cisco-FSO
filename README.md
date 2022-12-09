# Cisco-FSO

# Create an Intersight account - https://www.intersight.com/

- Start Trial

# Install Hashicorp Vault - Uses github account


# Create a Concourse account - https://concourse-ci.org/

1. https://concourse-ci.org/quick-start.html 

2.  Install in your environment

```bash
$ curl -O https://concourse-ci.org/docker-compose.yml
$ docker-compose up -d

```

3. Enter localhost:8080 into browser. test/test credentials

<img width="1148" alt="CleanShot-Google Chrome202212-09 at 14 38 20@2x" src="https://user-images.githubusercontent.com/9085386/206792042-4db1a2d1-bbf5-4bb0-a994-2c6bbca08f3f.png">

4. Next, install the fly CLI tool by downloading it from the web UI into your folder

![CleanShot-Google Chrome202212-09 at 15 03 13@2x](https://user-images.githubusercontent.com/9085386/206795852-05fb93b2-f6c7-4069-92ff-9e1131f3d8d3.png)

5. On Mac use cURL then connect Fly to concourse

```
$ curl 'http://localhost:8080/api/v1/cli?arch=amd64&platform=darwin' -o fly \
    && chmod +x ./fly && mv ./fly /usr/local/bin/

$ fly -t tutorial login -c http://localhost:8080 -u test -p test

```
