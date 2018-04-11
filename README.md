var CryptoJS = require('crypto-js');

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('XXX', '我六一儿童节。。。');

// Decrypt
var bytes = CryptoJS.AES.decrypt(ciphertext.toString(), '我六一儿童节。。。');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
