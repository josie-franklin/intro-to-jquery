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

`npm install jquery` or `npm i jquery`

The `package.json` file should have some new code in it. 

```
"dependencies": {
    "jquery": "^3.7.1"
}
```
There's also a whole new file that got generated, the `package-lock.json` file. It has pretty similar information to the package json.

These files tell npm what packages are needed to run a project, and at which versions. If someone clones your repo and runs the command `npm i` or `npm install`, the npm package manager will look at these files file and automatically install any packages at the correct versions needed. Pretty handy.

There's one more thing that was generated with that command, the `node_modules` directory. Taking a look in there reveals all of the code thet jQuery needs to run. Installing more packages would put more code in there. That folder can get pretty big, and we generally don't want to include with in our commits. Otherwise we would be commiting an immense amount of code, and it would be uneccesary code since we can just run the `npm i` command to get it back again. 

There's a way to let git know that we don't want a specific file included in our commit. Let's make a `.gitignore` file. 

On the first line,  type `node_modules`, and then save. You should see the node_modules directory grey out. Now, when you do a git commit, the node modules folder won't be commited. Nice. The `.gitignore` file is very common, we'll see it again another time. 

