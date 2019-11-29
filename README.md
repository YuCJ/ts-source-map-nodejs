# ts-source-map-nodejs

Run Node with `source-map-support`:

```sh
cd consumer
yarn
node -r source-map-support/register lib/index.js
```

The stdout should be:

```stdout
package run
Error: pacakge error line-4
    at Object.packageFunction [as packageFunc] (/Users/mac2016cjyu/Repos/ts-source-map-nodejs/consumer/node_modules/package/src/module.ts:3:9)
    at Object.<anonymous> (/Users/mac2016cjyu/Repos/ts-source-map-nodejs/consumer/src/index.ts:3:15)
    at Module._compile (internal/modules/cjs/loader.js:778:30)
    ...
```
