# TypeScript Lib Starter
Stater kit for modern TypeScript library. Generate JS ready to be published on npm.

## Clone the repo
`$ git clone git@github.com:fox1t/typescript-lib-starter.git`

`$ cd typescript-lib-starter`

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
