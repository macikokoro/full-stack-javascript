# Grunt

Once your local dev environment is set-up, it's a good idea to get started with Grunt. This is an extremely powerful JavaScript task runner, a build tool and and automation tool.

Some typical Grunt taks:

* Concatenation.
* Minification.
* Pre-processing Sass and Coffeescript.
* Image Optimization.
* Running tests.
* Starting a development Server.

**Installation:**

Global: `npm -g install grunt-cli`

Dev: `npm install grunt --save-dev`

Create a package.json file in your root directory with `npm init`

```text
//package.json
{
  "name": "my-project",
  "version": "0.0.1",
  "devDependencies": {
    "grunt": "~0.4.4"
  }
}
```

Create a Gruntfile.js

```text
module.exports = function(grunt) {

  // Project configuration.
  grunt.initConfig({
    simplemocha: {
      options: {
        timeout: 3000,
        ignoreLeaks: false,
        reporter: 'tap'
      },

      all: { src: ['test/**/*.js'] }
    },
    jshint: {
      all: ['Gruntfile.js','test/**/*.js']
    }
  });

  // Simplemocha test
  grunt.loadNpmTasks('grunt-simple-mocha');

  // JSHint
  grunt.loadNpmTasks('grunt-contrib-jshint');

  // Default task.
  grunt.registerTask('default', 'simplemocha');

};
```

`npm install` to install dependencies.

Here is an example of Grunt compiling SASS.

[grunt-sass-boilerplate](https://github.com/jqn/grunt-sass-boilerplate)

