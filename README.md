Taskmaster is a tool to help you create and assign tasks to your team easily and classy.
# [![Taskmaster Logo](http://www.elfwood.com/art/s/w/swiftcutter/ogre_taskmaster.jpg)](http://www.blueribbon-ti.com/) Taskmaster



## Prerequisites
* Node.js - Download and Install [Node.js](http://www.nodejs.org/download/). You can also follow [this gist](https://gist.github.com/isaacs/579814) for a quick and easy way to install Node.js and npm
* MongoDB - Download and Install [MongoDB](http://docs.mongodb.org/manual/installation/) - Make sure `mongod` is running on the default port (27017).
* Haraka  - Download and Install [Haraka] (http://haraka.github.io/) - Make sure haraka is running on the default port (587).


### Tools Prerequisites
* NPM - Node.js package manage; should be installed when you install node.js.
* Bower - Web package manager. Installing [Bower](http://bower.io/) is simple when you have `npm`:

```
$ npm install -g bower
```

### Optional [![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/)
* Grunt - Download and Install [Grunt](http://gruntjs.com).

## Additional Packages
* Express - Defined as npm module in the [package.json](package.json) file.
* Mongoose - Defined as npm module in the [package.json](package.json) file.
* Passport - Defined as npm module in the [package.json](package.json) file.
* AngularJS - Defined as bower module in the [bower.json](bower.json) file.
* Twitter Bootstrap - Defined as bower module in the [bower.json](bower.json) file.
* UI Bootstrap - Defined as bower module in the [bower.json](bower.json) file.

## Quick Install
  The quickest way to get started with MEAN is to install the `meanio` package from NPM.

  Install MEAN CLI:

    $ [sudo] npm install -g meanio@latest
    $ mean init <myApp>
    $ cd <myApp> && npm install

  We recommend using [Grunt](https://github.com/gruntjs/grunt-cli) to start the server:

    $ grunt

  If grunt aborts because of JSHINT errors, these can be overridden with the `force` flag:

    $ grunt -f

  Alternatively, when not using `grunt` you can run:

    $ node server

  Then, open a browser and go to:

    http://localhost:3000


## Troubleshooting
During install some of you may encounter some issues.

Most issues can be solved by one of the following tips, but if are unable to find a solution feel free to contact us via the repository issue tracker or the links provided below.

#### Update NPM, Bower or Grunt
Sometimes you may find there is a weird error during install like npm's *Error: ENOENT*. Usually updating those tools to the latest version solves the issue.

* Updating NPM:
```
$ npm update -g npm
```

* Updating Grunt:
```
$ npm update -g grunt-cli
```

* Updating Bower:
```
$ npm update -g bower
```

#### Cleaning NPM and Bower cache
NPM and Bower has a caching system for holding packages that you already installed.
We found that often cleaning the cache solves some troubles this system creates.

* NPM Clean Cache:
```
$ npm cache clean
```

* Bower Clean Cache:
```
$ bower cache clean
```

 
## Configuration


### Environmental Settings

 * __db__ - This is the name of the MongoDB database to use, and is set by default to __mean-dev__ for the development environment.
* __app.name__ - This is the name of your app or website, and can be different for each environment. You can tell which environment you are running by looking at the TITLE attribute that your app generates.
* __Social OAuth Keys__ - Facebook, GitHub, Google, Twitter. You can specify your own social application keys here for each platform:
  * __clientID__
  * __clientSecret__
  * __callbackURL__

To run with a different environment, just specify NODE_ENV as you call grunt:

    $ NODE_ENV=test grunt

If you are using node instead of grunt, it is very similar:

    $ NODE_ENV=test node server

> NOTE: Running Node.js applications in the __production__ environment enables caching, which is disabled by default in all other environments.

## Getting Started
We pre-included an article example. Check out:
  
  * [The Model](server/models/article.js) - Where we define our object schema.
  * [The Controller](server/controllers/articles.js) - Where we take care of our backend logic.
  * [NodeJS Routes](server/routes) - Where we define our REST service routes.
  * [AngularJs Routes](public/articles/routes/articles.js) - Where we define our CRUD routes.
  * [The AngularJs Service](public/articles/services/articles.js) - Where we connect to our REST service.
  * [The AngularJs Controller](public/articles/controllers/articles.js) - Where we take care of  our frontend logic.
  * [The AngularJs Views Folder](public/articles/views) - Where we keep our CRUD views.

## More Information
  * Visit us at [Blue Ribbon](http://www.blueribbon-ti.com).  

## License
[The MIT License](http://opensource.org/licenses/MIT)
