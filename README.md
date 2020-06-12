# Somersault


https://www.playframework.com/documentation/2.8.x/NewApplication

```sbt new playframework/play-scala-seed.g8```

## Heroku

- Add Procfile with web: run command must use $PORT as its set by Heroku
- Add system.properties with java runtime version https://devcenter.heroku.com/articles/java-support#supported-java-versions
- Set remote git dir to heroku master
- Heroku pipeline: local, review apps, staging (master), production (promoted from master)
- Work on a branch, make a PR - a new review app will be created with each PR and build each update
- Set heroku remote to the genearted app name for the PR to view logs.  See heroku console for build logs
- Merge to master.  Heroku will auto build the staging app.  Switch remote to view logs locally
- Promote to production by button click.
- TODO tests and CI gate the merge to master w/ Jenkins integration
- TODO log collection
- Set remote to heroku master.  Remote will change depending on which app to view logs

```$xslt
heroku git:remote -a somersault-p-staging-nzhvpdgxm
git remote -v
```

- change remote to staging after 

```$xslt
heroku git:remote -a somersault-staging
git remote -v
```


