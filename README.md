# RN CLI Maestro Sandbox

A simple "Hello World" React Native app for trying out testing with Maestro.

As of time of writing, Maestro is not succeeding on [GitHub Actions](https://github.com/CodingItWrong/RNCLIMaestroSandbox/actions).

## Requirements

- [Node](https://nodejs.org)
- [Yarn 1.x](https://classic.yarnpkg.com/lang/en/)
- [Ruby](https://www.ruby-lang.org/)
- [Cocoapods](https://cocoapods.org/)
- [Android Studio](https://developer.android.com/studio) and/or [Xcode](https://developer.apple.com/xcode/)
- [Maestro](https://maestro.mobile.dev/getting-started/installing-maestro)
- [Detox](https://wix.github.io/Detox/docs/introduction/getting-started#1-command-line-tools-detox-cli)

## Installation

- Clone the repo
- Run `yarn install`
- Run `cd ios && pod install`

Dependencies are locked with `yarn.lock`; please use `yarn` rather than `npm` for installing.

## Running

- In one terminal, run `yarn start`
- In another terminal, run `yarn android` or `yarn ios`

## E2E Tests

### Maestro

- First build and run the iOS app on a simulator
- Run `maestro test ./maestro/smoke-test.yml`

### Detox

- Run `detox build -c ios.sim.debug` (only needs to be run once per native code changes)
- Run `detox test -c ios.sim.debug`

## License

MIT
