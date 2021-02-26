# TypeScript Lib Starter ![TypeScript Lib Starter](https://user-images.githubusercontent.com/6388707/58274163-9204dc00-7d92-11e9-8746-6cd10e9aa9ea.png)

[![GitHub CI](https://github.com/fox1t/typescript-lib-starter/workflows/ci/badge.svg)](https://github.com/fox1t/typescript-lib-starter/actions)
[![TypeScript 4.0](https://img.shields.io/badge/TypeScript%20-4.0-blue.svg)](https://github.com/microsoft/TypeScript)
[![prettier](https://img.shields.io/badge/styled%20with-Prettier-blue.svg)](https://github.com/prettier/prettier)
[![ESLlint](https://img.shields.io/badge/linted%20by-ESLint-brightgreen.svg)](https://eslint.org)
[![node-tap](https://img.shields.io/badge/tested%20with-node--tap-green.svg)](https://github.com/tapjs/node-tap)

Starter kit for modern TypeScript libraries. Generates JavaScript ready to be published on npm.

 Batteries included. Period.
- [Prettier](https://prettier.io/) and [ESLlint](https://eslint.org) for formatting and linting
- [ts-node](https://github.com/TypeStrong/ts-node) for tests execution
- [node-tap](https://github.com/tapjs/node-tap) for testing and code coverage
- [tap-mocha-reporter](https://github.com/tapjs/tap-mocha-reporter) for test reporting
- [GitHub Actions](https://github.com/features/actions) configuration file for github actions workflow

## Clone the repo
`$ git clone git@github.com:fox1t/typescript-lib-starter.git {your_project_name}`

`$ cd {your_project_name}`

## Remove reference to this starter and re-init package.json
`$ rm -rf .git && git init && npm init`

## Install development dependencies
`$ npm i`

## Add remote origin and make initial commit
`$ git remote add origin git@github.com:{your_repository}.git`

`$ git add .`

`$ git commit -m "Initial commit"`

`$ git push -u origin master`

## Scripts
- `npm run build`: build TypeScript sources to dist directory
- `npm publish`: builds and publishes lib to [npmjs.com](https://www.npmjs.com)
- `npm test`: run tests in `./test` directory using [tap](https://www.npmjs.com/package/tap)
- `npm run test:watch`: watches `./src/` and `./test/` folders and restarts compilation and tests
- `npm run test:report`: saves test report to `out.tap` file
- `npm run test:reporter`: converts `out.tap` file to junit

## External typings augmentation
This starter is already configured to allow you to extend typings of external packages. The logic behind it is based on [this](https://www.typescriptlang.org/docs/handbook/declaration-files/templates/module-plugin-d-ts.html) official template. To augment a module, just create a folder with the same name as the module you are augmenting and add an index.d.ts in it. [Here](https://github.com/fox1t/fastify-websocket-router/tree/master/typings/fastify) you can find a real world example.

## Automatic Test and Code Coverage
Includes `azure-pipelines.yml` configuration file. You can build, test and publish code coverage on [Azure DevOps](https://docs.microsoft.com/en-us/azure/devops/organizations/public/?toc=%2Fazure%2Fdevops%2Forganizations%2Fpublic%2Ftoc.json&bc=%2Fazure%2Fdevops%2Forganizations%2Fpublic%2Fbreadcrumb%2Ftoc.json&view=azure-devops) for free with GitHub integration for OSS projects.

## Dev Dependencies

- `husky`: runs precommit `lint` hook
- `rimraf`: removes `lib` folder crossplatform
- `chokidar-cli`: file watcher
- `tap`: test runner
- `tap-mocha-reporter`: mocha reporter for tap
- `ts-node`: runs tests without compiling
- `prettier`
- `eslint`
- `eslint-config-prettier`: makes ESLint work nice with prettier
- `typescript`

## Spread the word
If you use this starter, add this badge to your project to help standardising TS library development.

`[![built with typescript-lib-starter](https://img.shields.io/badge/built%20with-typescript--lib--starter%20-blue.svg)](https://github.com/fox1t/typescript-lib-starter)`

[![built with typescript-lib-starter](https://img.shields.io/badge/built%20with-typescript--lib--starter%20-blue.svg)](https://github.com/fox1t/typescript-lib-starter)

## Node.js libraries built with TypeScript Lib Starter
- [fastify-flash](https://github.com/fastify/fastify-flash)
- [qs-to-mongo](https://github.com/fox1t/qs-to-mongo)
- [mongo-autoincrement](https://github.com/fox1t/mongo-autoincrement)
- [fastify-websocket-router](https://github.com/fox1t/fastify-websocket-router)

## License

MIT
