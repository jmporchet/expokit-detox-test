Expokit app that fails detox tests.

It's assumed you have a working development environment already setup (XCode, node, yarn, expo-cli, detox, etc.)

To get started enter the following commands:

`yarn`
`cd ios && pod install && cd ..` (that should take at least a few minutes)
`detox build`
`detox test` add the `--loglevel trace` flag for verbose output
