Initial Cloud Native application using Docker with an Express 

Quick Steps
$ npm install -g express-generator
$ express --view=pug namaari
$ cd namaari
$ npm install
$ DEBUG=namaari:* npm start

Additional Steps
To see which version of Express is in use:
$ npm list express

References for ExpressJS
* https://expressjs.com/
* https://expressjs.com/en/starter/installing.html
* https://expressjs.com/en/starter/generator.html
* https://www.npmjs.com/package/express-generator
* https://expressjs.com/en/guide/using-template-engines.html
* https://www.npmjs.com/package/pug

Troubleshooting Steps
> express: command not found
https://stackoverflow.com/questions/23002448/express-command-not-found


Since I'm using Express 4.x, I have not upgraded to using Express 5.x due to the Express Generator using Express 4.x (or so it seems to me).
For more information on Express 5.x, see https://expressjs.com/en/guide/migrating-5.html. 
To learn about Express 5.x, see https://expressjs.com/en/5x/api.html.

NPM

References for NPM
* https://docs.npmjs.com/cli/v8/commands/npx

Git

Remove "node_modules" directory that was mistakenly pushed to GitHub repo.
$ git rm -r --cached node_modules
$ git commit -m "remove the ignored directory node_modules"
$ git push origin main
* https://stackoverflow.com/questions/44168609/node-js-modules-pushed-to-github

Commit "package-lock.json" or not? Yes, commit.
* https://stackoverflow.com/questions/44206782/do-i-commit-the-package-lock-json-file-created-by-npm-5
