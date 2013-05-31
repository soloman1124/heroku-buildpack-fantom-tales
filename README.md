heroku-buildpack-fantom-tales
=============================

Heroku Buildpack for Tales based App (Fantom world).

It is a shameless copy of Slimer Dude's contribution:

    https://bitbucket.org/SlimerDude/heroku-buildpack-fantom

The following modifications are made to support [Tales](http://www.talesframework.org/) framework in Heroku:

* Install the Tales pod (http://repo.talesframework.org:9000) before executing *herokuPreCompile*. It is because Tales require *build.fan* to have *tales.pod* imported before executing, and therefore the *tales.pod* have to be installed first.
* Install the mysql java driver:

        mysql-connector-java-5.1.25-bin.jar
  
  so that the connection to mysql could work.




