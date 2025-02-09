Initial Cloud Native application using Docker with an Express 

> In a different world, maybe we could have been friends, but I have to do what's right for FANG. - Namaari

1. Create a NodeJS app.
2. To make app into a Cloud Native app, use CloudNativeJS to convert NodeJS app into a CloudNativeJS app.

## Quick Steps
```
# Install App via Express framework
# ----
$ npm install -g express-generator
$ express --view=pug namaari
$ cd namaari
$ npm install

# To see which version of Express is in use:
# ----  
$ npm list express

# Run App
# ----
$ npm start

# Run App in Debug Mode
# ----
$ DEBUG=namaari:* npm start
```

## References for ExpressJS
* https://expressjs.com/
* https://expressjs.com/en/starter/installing.html
* https://expressjs.com/en/starter/generator.html
* https://www.npmjs.com/package/express-generator
* https://expressjs.com/en/guide/using-template-engines.html
* https://www.npmjs.com/package/pug

## Troubleshooting Steps
[Solution for $ express: command not found](https://stackoverflow.com/questions/23002448/express-command-not-found)

## Express 4.x
Since I'm using Express 4.x, I have not upgraded to using Express 5.x due to the Express Generator using Express 4.x (or so it seems to me).
For more information on Express 5.x, see [https://expressjs.com/en/guide/migrating-5.html](https://expressjs.com/en/guide/migrating-5.html). 
To learn about Express 5.x, see [https://expressjs.com/en/5x/api.html](https://expressjs.com/en/5x/api.html).

## NPM References
* [https://docs.npmjs.com/cli/v8/commands/npx](https://docs.npmjs.com/cli/v8/commands/npx)

## Git
### Clone
* [https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls)

Remove "node_modules" directory that was mistakenly pushed to GitHub repo.
```
$ git rm -r --cached node_modules
$ git commit -m "remove the ignored directory node_modules"
$ git push origin main
```
* [https://stackoverflow.com/questions/44168609/node-js-modules-pushed-to-github](https://stackoverflow.com/questions/44168609/node-js-modules-pushed-to-github)

Commit "package-lock.json" or not? Yes, commit.
* [https://stackoverflow.com/questions/44206782/do-i-commit-the-package-lock-json-file-created-by-npm-5](https://stackoverflow.com/questions/44206782/do-i-commit-the-package-lock-json-file-created-by-npm-5)

# [CloudNativeJS](https://cloudnativejs.io/)
* Navigate to Docker. Was [here under CloudNativeJS](https://github.com/CloudNativeJS/docker), but now under [NodeShift here](https://github.com/nodeshift/docker).

Follow the steps with the [Docker Templates for NodeJS](https://github.com/nodeshift/docker?tab=readme-ov-file#docker-templates-for-nodejs)
```
$ wget https://raw.githubusercontent.com/CloudNativeJS/docker/master/Dockerfile
$ wget https://raw.githubusercontent.com/CloudNativeJS/docker/master/Dockerfile-tools
$ wget https://raw.githubusercontent.com/CloudNativeJS/docker/master/Dockerfile-run
```

# [Docker](https://www.docker.com/)
* [Get Started](https://docs.docker.com/get-started/)

## WGet
Verify WGet is installed.
```
$ wget --version
```

[Install WGet](https://formulae.brew.sh/formula/wget) from within Terminal, if not.
```
$ brew install wget
```

# References
[Dockerfile Basics](https://gist.github.com/mocon/0b567f77b693d73c41db5dcc6cacc8be)
