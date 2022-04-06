### TRC20 deploy

Guide: https://www.youtube.com/watch?v=wc4XN0SWvy4

`npm install -g tronbox`

`yarn global add pkgsign`

`npm view tronbox dist.tarball`
https://registry.npmjs.org/tronbox/-/tronbox-2.7.25.tgz

`wget https://registry.npmjs.org/tronbox/-/tronbox-2.7.25.tgz`

`yarn add @openzeppelin/contracts`

`pkgsign verify tronbox-2.7.17.tgz --package-name tronbox`

-   extracting unsigned tarball...
-   building file list...
-   verifying package...
-   package is trusted

`tronbox init`

`yarn add @openzeppelin/contracts`

`tronbox compile --compile-all`

`source .env && tronbox migrate --reset --network nile`

```
tron-trc20$ source .env && tronbox migrate --reset --network nile
Using network 'nile'.

Running migration: 1_initial_migration.js
  Deploying Migrations...
  Migrations:
    (base58) TWK2DA9VqCQHL4mXUhbKiHmHVQLpausucg
    (hex) 41df21d3a390da6e4c9376754ad521d2fbbe001d3b
Saving successful migration to network...
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Deploying LeoToken...
  LeoToken:
    (base58) TFN8JLBTYs6cyeyiZqKUL67VCoYALgC2iK
    (hex) 413b2e4555f39d5aec1a8dd56eaed525c4f9dc3fcf
Saving successful migration to network...
Saving artifacts...
```
