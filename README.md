# Somersault


https://www.playframework.com/documentation/2.8.x/NewApplication

```sbt new playframework/play-scala-seed.g8```

## Heroku

- Add Procfile with web: run command must use $PORT as its set by Heroku
- Set remote git dir to heroku master
- Create the app in Heroku dash

```$xslt
heroku git:remote -a somersault
```

- push to heroku master to deploy

```$xslt
git push heroku master
```




