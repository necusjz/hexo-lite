# HexoFWK
A snapshot for Hexo 3 using NexT 5 as its theme.

The specific version information is **Hexo 3.9.0** and **NexT 5.1.0**. It is a stable version with some UI configurations.

## Install
There are some dependencies, which need to be installed in advance.

### Node.js
We recommend installing a more compatible version: [10.20.0](https://nodejs.org/en/blog/release/v0.10.20/).

Under hexo-site, install the required packages in package.json:
```
{
  "name": "hexo-site",
  "version": "0.0.0",
  "private": true,
  "hexo": {
    "version": "3.9.0"
  },
  "dependencies": {
    "hexo": "^3.9.0",
    "hexo-deployer-git": "^1.0.0",
    "hexo-generator-archive": "^0.1.5",
    "hexo-generator-category": "^0.1.3",
    "hexo-generator-index": "^0.2.1",
    "hexo-generator-search": "^2.4.1",
    "hexo-generator-tag": "^0.2.0",
    "hexo-inject": "^1.0.0",
    "hexo-renderer-ejs": "^0.3.1",
    "hexo-renderer-marked": "^1.0.1",
    "hexo-renderer-stylus": "^0.3.3",
    "hexo-server": "^0.3.1"
  }
}
```

### Hexo
Once all the requirements are installed, you can install Hexo with npm:
```
$ npm install hexo-cli -g
```

## Usage
Generate static files and start a local server:
```
$ hexo generate
$ hexo server
```

Clean the cache and deploy your website:
```
$ hexo clean
$ hexo deploy
```

## Contributing
We love contributions! Before submitting a Pull Request, it's always good to start with a new issue first.

## License
This library is licensed under Apache 2.0. Full license text is available in [LICENSE](https://github.com/was48i/HexoFWK/blob/master/LICENSE).
