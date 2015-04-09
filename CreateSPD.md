## How to create the SPD ##

```
$ git clone git://github.com/certik/spd.git
$ cd spd
$ git co -b spd origin/spd
$ cd spkg/standard/
$ ./download_packages
$ cd ../../..
$ cp -a spd spd-3.4.2spd3
$ tar cf spd-3.4.2spd3.tar spd-3.4.2spd3
```

Now follow the [Installation](http://code.google.com/p/spdproject/wiki/Installation) howto.


## How to create a new SPD release ##


```
$ git clone git://github.com/certik/spd.git
$ cd spd
$ git co -b spd origin/spd
$ cd spkg/standard/
$ ./download_packages
$ vim sage_scripts/sage-banner  # edit the version & date in the banner
$ git ci -a -m "SPD version bumped to 3.4.2spd3"
$ git tag 3.4.2spd3
$ git push --tags git@github.com:certik/spd.git
$ cd ../../..
$ cp -a spd spd-3.4.2spd3
$ tar cf spd-3.4.2spd3.tar spd-3.4.2spd3
```

The relevant repositories are:

http://github.com/certik/spd

http://github.com/certik/spd_notebook