# Node.js

## Installation
* [Uninstall Node.js](http://stackoverflow.com/a/11178106/2510374)
* [Install Node.js globally with NVM](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-with-nvm-node-version-manager-on-a-vps)
* [Install npm packages globally on Linux without sudo](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo-linux.md)
* [node-and-npm-in-30-seconds.sh](https://gist.github.com/isaacs/579814)

## Learning
* [An Absolute Beginner's Guide to Node.js](http://blog.modulus.io/absolute-beginners-guide-to-nodejs)

### Modules

* npm outdated
* npm ls
* npm repo module_name
* [npm-shrinkwrap](https://www.npmjs.org/doc/cli/npm-shrinkwrap.html) - lock down dependency versions.

### Exceptions

* [Crash safety using domains in Node.js](https://engineering.gosquared.com/error-handling-using-domains-node-js)
* [domain.bind](http://nodejs.org/api/domain.html#domain_domain_bind_callback)(function(error, data) { ... })
* [domain.intercept](http://nodejs.org/api/domain.html#domain_domain_intercept_callback)(function(data) { ... })


## NPM Packages

### Create NPM packages

* [Creating and publishing a node.js module](http://quickleft.com/blog/creating-and-publishing-a-node-js-module)

## Troubleshooting

Sudo problems:
* ``sudo chown -R `whoami` ~/.npm``
* ``sudo chown -R `whoami` /usr/local/lib/node_modules``
* [NPM throws error without sudo](http://stackoverflow.com/questions/16151018/npm-throws-error-without-sudo)
