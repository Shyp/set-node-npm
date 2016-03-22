The script in this file is used to configure the correct versions of Node and
NPM across every project that the API depends on, instead of specifying a
version in each project.

To use this, add the following target to your Makefile:

```
circle-install:
	curl --remote-name https://raw.githubusercontent.com/Shyp/set-node-npm/master/set-node-npm
	chmod +x set-node-npm
	./set-node-npm
```
