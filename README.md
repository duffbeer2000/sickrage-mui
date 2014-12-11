This is a Dockerfile setup for sickbeard(non englisch series) - http://sickbeard.com/

To run:

```
docker run -d --name="sickbeard" -v /path/to/sickbeard/data:/config -v /path/to/downloads:/downloads -v /path/to/tv:/tv -v /etc/localtime:/etc/localtime:ro -p 8081:8081 duff/sickbeard
```

Edge
----
If you would like to run the latest updates from the master branch as well as enable in-app updates run:

```
docker run -d --name="sickbeard" -v /path/to/sickbeard/data:/config -v /path/to/downloads:/downloads -v /path/to/tv:/tv -v /etc/localtime:/etc/localtime:ro -e EDGE=1 -p 8081:8081 duff/sickbeard
```
