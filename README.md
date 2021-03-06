# sails-generate-scaffold

###**Note:** This module requires Sails **v0.10.0-rc8** or higher.

Base on the work of [irlnathan](http://github.com/irlnathan)

A `scaffold` generator for use with the Sails command-line interface.  A `scaffold` generates a rudimentary model, CRUD controller actions (e.g. index, new, create, edit, update, and destroy), and corresponding views of a Sails project.   The `scaffold` generator will also create a policy that enables flash messages for errors on the new and edit views. 

### To install:

```sh
$ npm install sails-generate-scaffold
```

Next open up the `.sailsrc` file located in the root of your sails project.  Add the `scaffold` by typing:

```javacript
{
  "generators": {
    "modules": {
    	"scaffold": "sails-generate-scaffold"
    }
  }
}
```

### To create a scaffold

##### On the command line

```sh
$ sails generate scaffold <a name for your scaffold> <optional: attributename:attributetype> <optional: --force>
```

Example:

```sh
$ sails generate scaffold user name:string age:integer email:email
```

The first argument will be the `model` and `controller` name.  You can add any number of model attributes and types. Finally, you can overwrite an existing scaffold by using the `--force` parameter.

### More Resources

- [Stackoverflow](http://stackoverflow.com/questions/tagged/sails.js)
- [#sailsjs on Freenode](http://webchat.freenode.net/) (IRC channel)
- [Twitter](https://twitter.com/sailsjs)
- [Professional/enterprise](https://github.com/balderdashy/sails-docs/blob/master/FAQ.md#are-there-professional-support-options)
- [Tutorials](https://github.com/balderdashy/sails-docs/blob/master/FAQ.md#where-do-i-get-help)
- <a href="http://sailsjs.org" target="_blank" title="Node.js framework for building realtime APIs."><img src="https://github-camo.global.ssl.fastly.net/9e49073459ed4e0e2687b80eaf515d87b0da4a6b/687474703a2f2f62616c64657264617368792e6769746875622e696f2f7361696c732f696d616765732f6c6f676f2e706e67" width=60 alt="Sails.js logo (small)"/></a>


### License

**[MIT](./LICENSE)**
&copy; 2017 [Brandon G. Neri](http://github.com/arcanite24) [irlnathan](http://github.com/irlnathan) & contributors

As for [Sails](http://sailsjs.org)?  It's free and open-source under the [MIT License](http://sails.mit-license.org/).

![image_squidhome@2x.png](http://i.imgur.com/RIvu9.png)
