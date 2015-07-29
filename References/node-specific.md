#NodeJS: Essentials

**REPL**
Through the node REPL (Read-Eval-Print Loop). In the same spirit as the Firebug or Web Inspector JavaScript consoles, this approach allows you to type in some JavaScript code, press Enter, and get it executed, right from your operating system’s command-line interface.

By executing node without any arguments from the command-line you will be dropped into the [REPL](https://nodejs.org/api/repl.html). It has simplistic  line-editing.

**NPM**

The Node Package Manager (NPM) allows you to easily manage modules in projects by downloading packages, resolving dependencies, running tests, and installing command-line utilities.

**NPM Custom Modules**

To define your own module, you need to create a package.json file.

In the directory created earlier (my-project), remove the node_modules directory and create a package.json with the following contents:

````javascript
{
      "name": "my-custom-project",
      "version": "0.0.1",
      "main": "./mymain"
      "dependencies": {
        "your dependencies": "0.5.0"
      }
}
````

The only required fields are name and version. Normally, modules have dependencies, which is an object that references other projects. The field **main** can be used to point out which file is that starting point of your module. With **npm install** you can install the local project. With **npm publish** you can, publish your project.

**NPM quick tricks**

You can install binary utilities by using the -g flag.

````
$ npm install -g myutilities
````

Also, you can use the NPM search feature to find a NPM package containing *meteor* in its name or description:

````
$ npm search meteor
````

To see the contents of its package.json, just run:

````
$ npm view *<package name>*
````
