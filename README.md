# About
*Amogus Client* is a custom Among Us client that uses [SkeldJS](https://github.com/SkeldJS/SkeldJS) for all of the protocol related things
# Building
To build the client, you need to use the `npm run build` with the arguments in this format:<br/>
`npm run build --<arch type> --<platform> <list of output types seperated by spaces>`<br/><br/>
*`arch type` - `x64` for 64-bit, `ia32` for 32-bit, `armv7l` for armv7l, and `arm64` for arm64*<br/>
*`platform` - `mac` for macos, `linux` for linux, and `win` for windows*<br/>
*`output type` - Any type of output type(dmg and pkg for macos, nsis for windows, deb, rpm, apk for linux, and zip is universal). A full list can be found in the specific target page for macos, windows, or linux [here](https://www.electron.build)*<br/>

Here is an example command to build a .dmg for macos: `npm run build x64 mac dmg`

The output will be in: `dist/<platform>/<arch type>`

For more information about command line arguments, check out the [electron-builder docs](https://www.electron.build/cli) ***WARNING: MAKE SURE TO IGNORE THE `--` THAT THE DOCUMENTATION PROVIDES. BUILD.JS PARSES THE ARGUMENTS WITHOUT THE `--`***

*Note: electron-builder package version is set to `22.10.4` because `22.10.5` causes an error when builing for macos*