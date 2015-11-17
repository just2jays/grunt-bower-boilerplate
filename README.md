# grunt-bower-boilerplate

### Get Grunt installed

Grunt...is installed on a per-project basis.
Grunt...needs Node and NPM. _Install it first!_

The _package.json_ file in the repo installs grunt for us.
Simply navigate to the project folder in Terminal and run the command:
```javascript
npm install
```

We should also install the Grunt CLI (command line interface) to give us global access to the grunt command from within Terminal.
```javascript
npm install -g grunt-cli
```
(-g = globally)

### Install base frameworks/libraries via Bower

The _bower.json_ file in the repo contains a list of frameworks and libraries we want to include in our project.
Initially it contains:
1. Bootstrap
2. jQuery
3. Modernizr

Feel free to add whatever other bower dependencies you wish to include here.

Once _bower.json_ has everything you want, simply run:

```javascript
bower install
```

### Install important/base Grunt plug-ins

Grunt makes development easier by running seemingly mundane tasks for you. (That is what it is after all by definition...a task runner)
Grunt knows what "plug-ins"(?) to load and what to do with them via the included _Gruntfile.js_ already in the repo.

The _Gruntfile.js_ comes with a handful of useful tasks ready to rock!
These are:

1. grunt-contrib-concat
	- used for concatenating multiple javascript files into a single javascript file
2. grunt-contrib-uglify
	- used for compressing javascript
3. grunt-contrib-sass
	- used for converting our sass files to plain 'ol css
4. grunt-contrib-watch
	- waits for you to change any javascript or css files, at which point it will automatically concat, compress, sassify, and save!

The last line of the _Gruntfile.js_ registers the default task(s) to run when the '_grunt_' command is issued via Terminal.
So lastly, go ahead and just run _grunt_ in your project root as:

```javascript
grunt
```

1. First (concat) concatenates the javascript files into a single .js file.
2. Then (uglify) compresses that file to shrink it down.
3. Then (watch) sits by waiting for you to start developing!


