heroku-buildpack-binaries
=========================

Heroku buildpack for Linux binaries


``` bash
$ echo https://s3.amazonaws.com/mybucket/server > .binaries
$ echo "web: bin/server" > Procfile
$ heroku create --stack cedar --buildpack https://github.com/vitalie/heroku-buildpack-binaries.git
```
