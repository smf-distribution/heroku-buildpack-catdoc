Heroku buildpack: catdoc
======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks)
for adding [catdoc](http://www.wagner.pp.ru/~vitus/software/catdoc/) to your application.

Multipacks
----------

Typically you'll want to use this with [multipack](https://github.com/ddollar/heroku-buildpack-multi),
like so:

    $ cat .buildpacks
    https://github.com/heroku/heroku-buildpack-nodejs.git
    https://github.com/leppert/heroku-buildpack-catdoc.git

    $ heroku config:add BUILDPACK_URL=git://github.com/ddollar/heroku-buildpack-multi.git
