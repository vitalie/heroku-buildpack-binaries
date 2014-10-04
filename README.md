heroku-buildpack-binaries
=========================

Heroku buildpack for Linux binaries


``` bash
$ echo https://s3.amazonaws.com/mybucket/server?7207e0a5d8a3af7b8e3f043b14078394 > .binaries
$ echo "web: bin/server" > Procfile
$ heroku create --stack cedar --buildpack https://github.com/vitalie/heroku-buildpack-binaries.git
$ git push heroku master
Initializing repository, done.
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 345 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)

-----> Fetching custom git buildpack... done
-----> Binaries app detected
-----> Found a .binaries file
       Getting https://s3.amazonaws.com/mybucket/server?7207e0a5d8a3af7b8e3f043b14078394
-----> Discovering process types
       Procfile declares types -> web

-----> Compressing... done, 2.3MB
-----> Launching... done, v4
       http://nameless-savannah-7843.herokuapp.com/ deployed to Heroku

```


Credits
-------

- Pete Keen (@peterkeen)
