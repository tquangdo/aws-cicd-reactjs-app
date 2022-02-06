# aws-cicd-reactjs-app 🐳

![Stars](https://img.shields.io/github/stars/tquangdo/aws-cicd-reactjs-app?color=f05340)
![Issues](https://img.shields.io/github/issues/tquangdo/aws-cicd-reactjs-app?color=f05340)
![Forks](https://img.shields.io/github/forks/tquangdo/aws-cicd-reactjs-app?color=f05340)
[![Report an issue](https://img.shields.io/badge/Support-Issues-green)](https://github.com/tquangdo/aws-cicd-reactjs-app/issues/new)

![overview](screenshots/overview.png)

## reference
[youtube](https://www.youtube.com/watch?v=zkNdHv1iMgY)

## local
### A) test
```shell
yarn test
=>
Test Suites: 2 passed, 2 total
Tests:       2 passed, 2 total
Snapshots:   0 total
Time:        2.932s
```
- edit `src/components/Root/Counter/Counter.js`
```js
dispatch(-200) // OK: dispatch(-2)
```
- test again
```shell
yarn test
=>
Test Suites: 1 failed, 1 passed, 2 total
Tests:       1 failed, 1 passed, 2 total
Snapshots:   0 total
Time:        2.796s
```
### B) run
```shell
yarn install && yarn watch
```
- access `http://localhost:1234/` on browser
![local](screenshots/local.png)

## AWS
### 1) CodePipeline
- create name=`DTQPipelineReactJS`