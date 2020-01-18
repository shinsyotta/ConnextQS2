A very simple example app using Connext.


Clone the app, and install the node packages with...
`npm install`

Then start the app using...
`npm start`

Might have to upgrade eccrypto dependency separately.
```
cd node_modules/eccrypto
npm run install
```

## Docker mode

If the following does work for whatever reason, try running this app in Docker!

The only prerequisite is [installing docker](https://docs.docker.com/docker-for-mac/install/).

```
npm run build
```

This will build the docker image according to recipe outlined in Dockerfile.

```
npm run start-docker
```

This will execute the docker image. It includes the flag `--mount=type=bind,source=`pwd`/src,target=/root/src` which mounts the `src` folder into the docker image. This means we don't need to rebuild the image every single time the source code changes (Ditto for the .env file).

Address: 0x55fc4b71A866ce26c888fDEC5413840EAFA34643
BIP32 Extended Public Key, a.k.a. xPub: xpub6EWHGJjmU9BqgVHnrqxG9qZHFe1UZkPLboL2varSg4ouMz8YoY7m3Wr9sPaPc4rVGVspr8y52z8kxSWJfVNxGccWmum8Bc1UipuCrdeZFBQ
