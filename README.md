# UTP


## Usage notes

1. Clone
```
git clone https://github.com/lisatwyw/UTP/
```

2. Build: 
```
cd UTP
export DOCKERID=<your docker id>
docker image build --tag $DOCKERID/utp:1.0 .  

# notes: period after whitespace and lowercase when spelling utp
```

```
docker build -t utp .
```


3. Run: 
```
docker container run --detach -p 80:80 $DOCKERID/utp:1.0

# p for publish 
```


## Try it

1. Try repeat above at [Docker classroom](https://training.play-with-docker.com/beginner-linux/). 

2. Find the link '''Click here to load the website'''; it should have URL like this:
http://ip172-19-0-37-chok4tbqes6000cn7shg-8080.direct.labs.play-with-docker.com/

3. After waiting for the server, you should hopefully see a webpage displayed:
![Screenshot 2023-05-26 at 16-36-36 Screenshot](https://github.com/lisatwyw/UTP/assets/38703113/7fdbe77a-2dc0-4aeb-a108-16e7ba9703e4)

Last tested May 26, 2023

# References  

- [DockerSamples](https://github.com/dockersamples/linux_tweet_app/tree/master)
- [Docker image examples](https://github.com/techiescamp/docker-image-examples) 
