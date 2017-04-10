### Linting with eslint!

Having clean, well formatted, and consistent code is important. A linter is a tool that helps up stay consistent!

The most popular linting tool for javascript is [eslint](http://eslint.org/). It is highly configurable and easy to use. There are also many style guides that companies and people make available that are extremely thorough.

Here is a list of some of the more popular style guides
- [airbnb](https://www.npmjs.com/package/eslint-config-airbnb)
- [standard](https://github.com/feross/eslint-config-standard)
- [semistandard](https://github.com/Flet/eslint-config-semistandard)
- [google](https://github.com/google/eslint-config-google)
- [many more!](http://lmgtfy.com/?q=eslint+style+guides)

You can also define your own rules and create your own style guide!

###Setup
There are a few steps we need to do to get our linter up and running.

- Find a style guide that you want to use!
- Install eslint in your project directory
- Install the ```eslint-config``` and its dependencies for the style guide you want to use
- Create a ```.eslintrc.json``` file for our eslint configuration
- Create a ```.eslintignore``` file so we can ignroe files that we want to (works just like ```.gitignore```)
- In ```.eslintrc``` extend eslint to use the config we installed
- Add a lint script to package.json ```"lint": "./node_modules/.bin/eslint ./"``` Note: we are targeting the current directory
- Run the script with a ```-s``` flag so that npm will not throw errors
- ```npm run lint -s```
