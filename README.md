This plugin add a gradle script to remove arm64-v8a libs, since android cannot load 32- and 64-bit native libraries concurrently.
That means if you at least one ARM64 native lib, android wont load ARM32 libs. Hence your app will crash.

cordova plugin add cordova-plugin-remove-arm64 --save