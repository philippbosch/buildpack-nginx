# Nginx Buildpack
## w/ Grunt

**Note**: This has only been tested with [dokku](https://github.com/progrium/dokku) - it may not work elsewhere.

## Structure
* Gruntfile.coffee - File: its presence signals that this buildpack should be used
* nginx.conf.erb - Optional File: overrides `conf/nginx.conf.erb`
* mime.types - Optional File: overrides `conf/mime.types`


This buildpack expects a grunt task `dist` that should generate a directory `dist` with
all files that Nginx shall serve.


Based on [buildpack-nginx](https://github.com/rhy-jot/buildpack-nginx) by [rhy-jot](https://github.com/rhy-jot).
