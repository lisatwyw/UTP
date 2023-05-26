# UTP


## Usage notes

1. Clone
```
git clone https://github.com/lisatwyw/UTP/
```

2. Build: 
```
cd UTP
export $DOCKERID=<your docker id>
docker image build --tag $DOCKERID/utp:1.0 .  

# notes: period after whitespace and lowercase when spelling utp
```

```
docker build -t utp .
```


3. Run: 
```
docker container run --detach -p 80:80 utp

# p for publish 
```



# References  

- [DockerSamples](https://github.com/dockersamples/linux_tweet_app/tree/master)
- [Docker image examples](https://github.com/techiescamp/docker-image-examples) 
