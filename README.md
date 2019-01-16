# Testing upgrading from `npm-shrinkrap.json` to `package-lock.json`

This repo demonstrates upgrading from npm3 with a `npm-shrinkwrap.json` file to npm6 with a `package-lock.json`.

### Notes

1. The `left-pad` package at v1.2 (not the latest version) was installed with npm3
2. A `npm-shrinkwrap.json` file was created with npm3
3. The `npm3_node_modules` directory is the installed `node_modules` directory after installing
4. Then `npm install` was run again with npm6, with no `node_modules` dir. A warning about the `npm-shrinkwrap.json` file is observed in the console
5. The `npm6_shrinkwrap_node_modules` directory is the installed `node_modules` directory after installing
6. The `npm-shrinkwrap.json` is renamed to `package-lock.json`
7. Then `npm install` is run again, with no `node_modules` dir. No warning about the `package-lock.json` is observed
8. The `npm6_package_lock_node_modules` directory is the installed `node_modules` directory after installing
