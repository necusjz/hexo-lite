# Hexo Lite
Lite version of Hexo with several UI configurations.

The specific version information is **Hexo 3.9.0** and **NexT 5.1.0**.

## Installation
There are several prerequisites that need to be installed in advance.

### Node.js
We recommend installing a more compatible version [10.24.1](https://nodejs.org/en/blog/release/v10.24.1):
```bash
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 10

# Verify the Node.js version:
node -v # Should print "v10.24.1".
nvm current # Should print "v10.24.1".

# Verify npm version:
npm -v # Should print "6.14.12".
```

Under hexo-site, install the required packages in `package.json`:
```json
{
  "name": "hexo-lite",
  "version": "1.0.0",
  "private": true,
  "hexo": {
    "version": "3.9.0"
  },
  "dependencies": {
    "hexo": "^3.9.0",
    "hexo-abbrlink": "^2.2.1",
    "hexo-cli": "^1.0.4",
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

## Usage
Create a new post:
```bash
$ hexo new <title>
```

Generate static files and start a local server:
```bash
$ hexo generate
$ hexo server
```

Clean the cache and deploy our website:
```bash
$ hexo clean
$ hexo deploy
```

## Contributing
We love contributions! Before submitting a Pull Request, it's always good to start with a new issue first.

## License
This repository is licensed under MIT. Full license text is available in [LICENSE](https://github.com/necusjz/hexo-lite/blob/main/LICENSE).
