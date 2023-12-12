Contains Support for every Language text encryption.

### Usage

1. Include `Encoder_Decoder.min.js` in your project file's <Head> Tag.
2. In JavaScript code of your website project, use the function `Encode()` to encrypt a String & function `Decode()` to decrypt an encrypted string.
## For Example

```
const EncodedString = Encode("My Secret String");
const DecodedString = Decode(EncodedString);
```

### Config

In Version 1.0 You can only change names of functions for now, like if you already have declared a function named `Encode()` or `Decode()`, then you can change these Functions names from the file `Encoder_Decoder.min.js`

### Debugging

In Version 1.0 You can debug these functions executing time, like to check if they are capable to work with your project or not.

**To debug:**

```
const TextData = "My Secret String";
var start = Date.now();
const EncodedString = Encode(TextData);
let tt1 = Date.now() - start;
var start = Date.now();
const DecodedString = Decode(EncodedString);
let tt2 = Date.now() - start;
console.log('Encrypted Version:' + EncodedString);
console.log('Decrypted Version: ' + DecodedString);
console.log('Encryption TimeTaken:' + tt1 + 'ms');
console.log('Decryption TimeTaken: ' + tt2 + 'ms');
```

### Handling Errors

1. If sometime the `Encode()` function do not receives any String, then It will consider it `undefined`
2. Also same for `Decode()` that if it receives something that is not able to decrypt or decode then it returns empty string.
3. If `Encode()` receives data other than a string then it will not produce any kind of error, but for `Decode()` function, this can cause error.

### Disclaimer

This JavaScript Program uses [LZ-String](https://github.com/pieroxy/lz-string) & adds some important features in it to enhance performance & program efficiency.
These functions are not tested completely on all browsers & systems, So to say that they are error proof or not is difficult, but check other versions if you want error proof functions.
