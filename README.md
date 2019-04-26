Expokit app that fails detox tests.

It's assumed you have a working development environment already setup (XCode, node, yarn, expo-cli, detox, etc.)

# Getting started

To get started enter the following commands:

`yarn`
`cd ios && pod install && cd ..` (that should take at least a few minutes)
`expo start` to start the bundler
`detox build`
Launch Simulator.app and choose the correct device (Hardware > Device > iOS 12.1 > iPhone 7 as setup in `package.json`)
`detox test`, and add the `--loglevel trace` flag for verbose output

# Repo status

This repo has been created with:
`expo init`
`expo eject` choosing the expokit option
`yarn add -D detox jest`
`cd ios && pod install && cd ..`
configure `package.json` according to the docs at https://github.com/wix/Detox/blob/master/docs/Introduction.GettingStarted.md and https://github.com/wix/Detox/blob/master/docs/Guide.Jest.md. Expokit uses workspaces so I needed to customize that step.
`detox init -r jest`

# Trace file

The trace log output has been stored in `trace.txt` via `detox test --loglevel trace > trace.txt`
