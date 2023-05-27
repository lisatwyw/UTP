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
[Last tested May 26, 2023]

1. Try repeat above at [Docker classroom](https://training.play-with-docker.com/beginner-linux/). 

2. Find the link '''Click here to load the website'''; it should have URL like this:
http://ip172-19-0-37-chok4tbqes6000cn7shg-8080.direct.labs.play-with-docker.com/

3. After waiting for the server, you should hopefully see a webpage displayed:
![Screenshot 2023-05-26 at 16-36-36 Screenshot](https://github.com/lisatwyw/UTP/assets/38703113/7fdbe77a-2dc0-4aeb-a108-16e7ba9703e4)

 


## Level up
[Last tested May 26, 2023]

Try more advanced example written by [Xavier Vasques](https://towardsdatascience.com/build-and-run-a-docker-container-for-your-machine-learning-model-60209c2d7a7f)

1. Clone
```
$ git clone https://github.com/xaviervasques/EEG-letters.git
$ cd EET-letters
```

2. Build (includes pip installations and training using ```train.py```)
```
docker build -t docker-ml-model -f Dockerfile .
```
 
3. Test on new data by calling ```inference.py```
```
docker run docker-ml-model python3 inference.py
```



# References  

- [DockerSamples](https://github.com/dockersamples/linux_tweet_app/tree/master)
- [Docker image examples](https://github.com/techiescamp/docker-image-examples) 
- ['''A quick and easy build of a Docker container with a simple machine learning model''' by Xavier Vasque](https://towardsdatascience.com/build-and-run-a-docker-container-for-your-machine-learning-model-60209c2d7a7f)
