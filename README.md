Expokit app that fails detox tests.

It's assumed you have a working development environment already setup (XCode, node, yarn, expo-cli, detox, etc.)

To get started enter the following commands:

`yarn`
`cd ios && pod install && cd ..` (that should take at least a few minutes)
`expo start` to start the bundler
`detox build`
`detox test`, and add the `--loglevel trace` flag for verbose output

The trace log output has been stored in `trace.txt` via `detox test --loglevel trace > trace.txt`
