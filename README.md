# TypeScript Lib Starter    [![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
Stater kit for modern TypeScript library. Generate JS ready to be published on npm.

## Clone the repo
`$ git clone git@github.com:fox1t/typescript-lib-starter.git {your_project_name}`

`$ cd {your_project_name}`

## Remove reference to the original starter
`$ rm -rf .git && git init && npm init`

## Install development dependencies
`$ npm i`

## Scripts
- `npm run build`: build TypeScript sources to lib directory
- `npm publish`: builds and publishes lib to [npmjs.com](https://www.npmjs.com)
- `npm test`: run tests inside `./test` directory using [tap](https://www.npmjs.com/package/tap)
- `npm run test:watch`: watches `src/` and `test/` folders and restarts compilation and tests
- `npm run test:report`: saves test report to `out.tap` file
- `npm run test:reporter`: converts `out.tap` file to junit

## External typings augmentation
This starter is already configured to allow you to extend typings of external packages. The logic behind it is based on [this](https://www.typescriptlang.org/docs/handbook/declaration-files/templates/module-plugin-d-ts.html) official template. To augment a module, just create a folder with the same name as the module you are augmenting and add an index.d.ts in it. [Here](https://github.com/fox1t/fastify-websocket-router/tree/master/typings/fastify) you can find  a real world example.

## Dev Dependencies

- `cross-env`: sets TS_NODE_PROJECT for running tests with tap/ts-node crossplatform
- `husky`: runs precommit `lint` hook
- `rimraf`: removes `lib` folder crossplatform
- `chokidar-cli`: file watcher
- `tap`: test runner
- `tap-mocha-reporter`: mocha reporter for tap
- `ts-node`: runs tests without compiling
- `prettier`
- `tslint`
- `tslint-config-prettier`: makes tslint work nice with prettier
- `typescript`

## License

MIT
