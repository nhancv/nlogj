# nlogj
![npm](https://img.shields.io/npm/v/nlogj.svg) ![license](https://img.shields.io/npm/l/nlogj.svg) ![github-issues](https://img.shields.io/github/issues/nhancv/nlogj.svg)

Awesome nodejs log to file

[![nodei.co](https://nodei.co/npm/nlogj.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/nlogj)

## Installation
```
npm install nlogj --save
```

## Usage
```
const logFile = require('nlogj')

logFile
	.setTag('Test')
	.setLogName('hello.log')
	.setLogDir(__dirname)
	.clearLog()
	.log('hello')
	.log('hello2')

 ```

You will see a new log file with name `hello.log` in current folder with content
```
2018-02-11 16:04:23 [Test]: hello
2018-02-11 16:04:23 [Test]: hello2
```