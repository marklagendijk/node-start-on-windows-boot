# node-start-on-windows-boot
Simple utility to enable / disable starting a program on Windows boot, by modifiying the right registry values.

## Example
``` javascript
var startOnBoot = require('start-on-windows-boot');

startOnBoot.enableAutoStart('MyApplication', 'C:\\Program Files\\MyApplication\\MyApplication.exe');
```

## Docs

### enableAutoStart(name, file, callback)
Adds the auto-start registry record of a program.

#### name
Type: `string`

The name of the program.

#### file
Type: `string`

The full path of the programs' executable.

#### callback
Type: `Function`

Optional callback function.

### disableAutoStart(name, callback)
Removes the auto-start registry record of a program.

#### name
Type: `string`

The name of the program.

#### callback
Type: `Function`

Optional callback function.

### getAutoStartValue(name, callback)
Gets the value of the auto-start registry record of a program.

#### name
Type: `string`

The name of the program.

#### callback
Type: `Function`

The callback which gets called with the value (and a error, if any).



