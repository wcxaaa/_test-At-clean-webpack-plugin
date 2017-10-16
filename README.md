# _test-At-clean-webpack-plugin
investigation of issue johnagan/clean-webpack-plugin#59

To make clean-webpack-plugin or rimraf complain, after `npm install`, you can just run `npm run build` , `npm run serve` and once again `npm run build`. 

[Clean-webpack-plugin](https://github.com/johnagan/clean-webpack-plugin) now throws an error as displayed in this issue. Additionally, running `npm run clear` right now to initiate [rimraf](https://github.com/isaacs/rimraf) cleaning throws a similar error as well:

> Error: ENOTEMPTY: directory not empty, rmdir 'dist'