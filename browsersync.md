# Auto refreshing with Browsersync

<iframe width="725" height="408" src="https://www.youtube.com/embed/JCZIbd_LtMY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Installation

Ensure `node` and `npm` are installed. Instructions are in the Getting setup guide.

```bash
node --version
# v11.12.0

npm --version
# 6.9.0
```

Note: Your version numbers may be different.

```bash
npm init -y
npm install browser-sync
```

You may get errors to the screen in either case, but the application may still have installed. To verify browser-sync is installed, run this command:

```bash
./node_modules/.bin/browser-sync --version
```

You should see version number, something like `2.26.3` (although it may be different). If you see anything other than a version number, the application likely did not install correctly. Due to the complex configuration of each installation of Mac OS, unfortunately I am not able to debug every situation. browser-sync is a helpful tool in developing websites, but it is not a absolute requirement for this course. So it is okay to continue on with the assignments and tutorials with hitting Command+R to refresh the browser every time you make a change to the HTML, CSS (and eventually javascript) files.

## Starting a server

The power of Browsersync is it can start a local webserver (will be important later in this course) and watch for file changes. When ever you save a file, it will automatically update the preview of your webpage with those changes.

Edit the `package.json` file to include a 'start' script

```json{3}
...
"scripts": {
  "start": "./node_modules/.bin/browser-sync  start --server --files='**/*'",
  "test": "echo \"Error: no test specified\" && exit 1"
},
...
```

Run the `npm start` command

```bash
npm start
```

The output will look something like this:

```
> git-example@1.0.0 start /Users/nickdenardis/Sites/imt-549/git-example
> browser-sync  start --server --files='**/*'

[Browsersync] Access URLs:
 -----------------------------------
       Local: http://localhost:3000
    External: http://10.10.10.1:3000
 -----------------------------------
          UI: http://localhost:3001
 UI External: http://localhost:3001
 -----------------------------------
[Browsersync] Serving files from: ./
[Browsersync] Watching files...
```

## Visit the local webserver

Alt+Click on the URL or visit [http://localhost:3000/](http://localhost:3000/) in Chrome to view your website.

It will start the server in the directory you run the command and try to open the index.html in the same directory the command is run. If there is no index.html in the same directory, you will see a Cannot GET / error.

If you have files in folders, you will need to manually type that folder (it will likely be case-sensitive) into the URL.

## Opening an index file in a folder

Imagine you have a directory that looks like this:

```bash
| index.html
| README.md
| .gitignore
| coffee
| |____index.html
| |____css
| | |____styles.css
| |____images
| | |____...
```

The "coffee/index.html" file would be visible in a browser at: [http://localhost:3000/coffee/](http://localhost:3000/coffee/)

## Stopping the server

Use the Control+C key combination in the terminal to stop the server.

```bash
^C
```

## Resources

- [Browsersync command line options](https://browsersync.io/docs/command-line)
- [Basic example of Browsersync 'start' command](https://scotch.io/tutorials/how-to-use-browsersync-for-faster-development)