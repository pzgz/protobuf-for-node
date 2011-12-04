Please check [here](https://code.google.com/p/protobuf-for-node/) for detail. I forked this repository from there, and make some changes to make it work with the latest node.js version, which is 0.6.4.

After the changes, I have successfully made compile on Mac OS X 10.7. More tests need to be done on other linux platforms.

## Build

To successfully make a build, you will need to run following:

```
PROTOBUF=<protobuf prefix> /path/to/node/bin/node-waf configure clean build
```

In my case (Mac OS X Lion 10.7), I ran following scripts:

```
PROTOBUF=/usr/local/Cellar/protobuf/2.4.1/ node-waf configure 
```

Make sure you have compliled and install protobuf from google.