Groestlcoin Core RPC Auth Generator
=====================================

What is this tool?
----------------

Anyone who runs software that needs to talk to their own Groestlcoin Core node will need to configure that node to allow RPC access with the appropriate authentication. Groestlcoin Core's rpcauth option requires the value to be in the form of: [username]:[saltedhashedpassword]

This tool makes it easier for users who are unfamiliar with running command line scripts to create the salted, hashed password value.

Who needs this tool?
----------------
Groestlcoin wallet developers may find this tool helpful to quickly generate credentials.

Groestlcoin users who run Lightning Network nodes need to be able to configure the lightning node to talk to the Groestlcoin node.

Building
-------
Install browserify: http://browserify.org/
run from the js/ directory:
npm install
browserify -e rpcauth.js -o browserified.js -t [ babelify --presets [@babel/preset-env] ]

License
-------

The Groestlcoin Core RPC Auth Generator is released under the terms of the MIT license. See [LICENSE](LICENSE) for more
information or see http://opensource.org/licenses/MIT.
