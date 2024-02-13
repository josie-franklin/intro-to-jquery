# intro-to-jquery

Lets get familiarized with the npm package manager and a popular library, jQuery.
## Prerequisites
- Node.js
- npm (comes with the node install package)

## npm

Installing npm to your repo

- Open a terminal in the root of your repo
- Run the command `npm init`
- Answer the questions that appear, or just hit `enter` to use the defaults. You can avoid this by running `npm init -yes` to automatically use the default answers.

Your repo should now have a file named `package.json` in your root directory. Feel free to take a look at what's in there. There's an object that contains many properties that describe your project. Neat. 

We can install a package using npm. Check out the npm webpage https://www.npmjs.com/ to look at what's out there. We'll be installing the jQuery https://jquery.com/ package, a popular library for JavaScript DOM manipulation. It's very common and well-maintained, with more ways to use it than just npm. This time we'll just run the command on their npm page to install it. https://www.npmjs.com/package/jquery

`npm i jquery`

The `package.json` file should have a new line in it. 

```
"dependencies": {
    "jquery": "^3.7.1"
}
```