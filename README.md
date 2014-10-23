Heroku buildpack for imagemagick built with libwebp
=======================

Usage
-----
To use this buildpack, you should prepare .buildpacks file that contains this buildpack url and your real buildpack url.  

    $ cat .buildpacks
    https://github.com/nrj/heroku-buildpack-imagemagick-webp.git
    https://github.com/heroku/heroku-buildpack-nodejs.git 

The first build pack is the git URL to this repo.
The second build pack is for a NodeJS app, see [https://github.com/heroku](https://github.com/heroku) for other app build packs.
    
    $ heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git
    
    $ git push heroku master
    ...