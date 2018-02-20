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

The application will also be deployed on Multiple platforms.

This will solidify someone's grasp over Webpack.

Cheers,

[Raj](https://twitter.com/rja907)
