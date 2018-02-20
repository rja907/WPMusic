# Music

An app that uses Webpack for Vendor Asset Caching, Vendor Splitting, Code Splitting and Chunk Hashing for Cache Busting.

Repo workflow:

`Make changes in the webpack.config.js file to bundle js files.`

`Make changes in the webpack.config.js file to bundle css files.`

`Run 'npm run build'.`

`Vendor Caching using CommonsChunkPlugin!`

`Run 'npm i --save-dev html-webpack-plugin'.`

`Make changes in webpack.config.js.`

`Move index.html to the src directory from the root directory.`

`Remove the script tag of index.html because html-webpack-plugin will do that for us.`

`Run 'npm run build'.`

`Added chunkhash so that outdated files are not rendered via cache.`

`Now every time we build, we'll find a different hash code. So, the cached version(outdated) will not be loaded.`

`We can check the dist/index.html to see that the updated build files are sourced.`

`We can see that our build folder looks messy with multiple build files. That needs to change!`

`Run 'npm i --save-dev rimraf'. This will help clean project build files.`

`Add script 'clean' to package.json so that rimraf cleans the dist folder.`

`Run 'npm i --save-dev webpack-dev-server@2.2.0-rc.0'.`

`Add script 'serve' to package.json so that webpack-dev-server serves files.`

`Run 'npm run serve'.`

`Change one file. (I changed index.js from src) to see that the w-d-s takes almost negligible time to serve the new file.`

`Make changes in router.js to add code splitting of react routes.`

`To be ready for deployment we add 'NODE_ENV=production' to the "build" script of package.json.`

`To make a production ready build (includes minification etc.), we add '-p' after webpack in the build script.`

`Run 'npm run build'.`

The application will also be deployed on Multiple platforms.

This will solidify someone's grasp over Webpack.

Cheers,

[Raj](https://twitter.com/rja907)
