# hexo-deployer-heroku

[![Build Status](https://travis-ci.org/hexojs/hexo-deployer-heroku.svg?branch=master)](https://travis-ci.org/hexojs/hexo-deployer-heroku)
[![NPM version](https://badge.fury.io/js/hexo-deployer-heroku.svg)](https://www.npmjs.com/package/hexo-deployer-heroku)
[![Coverage Status](https://coveralls.io/repos/hexojs/hexo-deployer-heroku/badge.svg)](https://coveralls.io/r/hexojs/hexo-deployer-heroku)
[![Build status](https://ci.appveyor.com/api/projects/status/github/hexojs/hexo-deployer-heroku?branch=master&svg=true)](https://ci.appveyor.com/project/tommy351/hexo-deployer-heroku/branch/master)

Heroku deployer plugin for [Hexo].

## Installation

``` bash
$ npm install hexo-deployer-heroku --save
```

## Options

You can configure this plugin in `_config.yml`.

``` yaml
# You can use this:
deploy:
  type: heroku
  repo: <repository url>
  message: [message]
  include_hidden: false
  static_json: <static.json file path>
```

- **repo**: Repository URL.
- **message**: Commit message. The default commit message is `Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}`.
- **include_hidden**: Include hidden files (starting with `.`) when copying from the source.
- **static_json**: Path to the custom `static.json` file that will overwrite the default if given.

## Reset

Remove `.deploy_heroku` folder.

``` bash
$ rm -rf .deploy_heroku
```

## License

MIT

[Hexo]: http://hexo.io/