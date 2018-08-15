

# CLI tool for the Udacity Reviews API

`urcli` is a Command Line Interface for configuring and running API calls against the Udacity Reviews API.

[![npm downloads](https://img.shields.io/npm/dt/urcli.svg?style=flat)](https://www.npmjs.com/package/urcli)
[![npm version](https://img.shields.io/npm/v/urcli.svg?style=flat)](https://www.npmjs.com/package/urcli)
[![npm license](https://img.shields.io/npm/l/urcli.svg?style=flat)](https://www.npmjs.com/package/urcli)

---
**IMPORTANT NOTICE:** The Udacity Reviews API has been shut down. `urcli` no longer works and this repo has been archived. Thanks to everyone who contributed with code and ideas! 

---
## Requirements
- [Node.js](https://nodejs.org/en/download/) v6.0.0 or higher
- NPM (v3.0.0+ recommended) (this comes with Node.js)

## :zap: Quickstart

1. Run `npm install -g urcli`.
2. Get a new token from the API Access link in the [Reviewer Dashboard](https://review.udacity.com/#!/submissions/dashboard). <img src="http://i.imgur.com/QH7onbk.png" alt="Token retrieval" width="500px">
3. Run `urcli setup`. When prompted, paste in the token you just got and then go through the rest of the setup.
4. Run `urcli assign` proceeded by valid project ids for projects you are certified for. Ex:
    - `urcli assign 145`, places you in the queue for project 145.
    - `urcli assign 134 145 46`, places you in the queues for project 145, 134 and 46.
    - `urcli assign all`, places you in the queue for every project you are certified for.
5. Profit! (literally).

## Upgrade

2. Get a new token (See Quickstart #2).
1. Press `ESC` to stop the currently running instance (If you have urcli running).
3. Run `npm i -g urcli`.
4. Run `urcli setup`.
5. Run your assign command, `urcli assign all`.

## Executables

If you don't know how to use Node and npm, you can use the [executables](https://github.com/trolster/urcli/releases) instead. See the [wiki entry](https://github.com/trolster/urcli/wiki/Executables) for more.

## Documentation

Documentation can be found in the [Wiki](https://github.com/trolster/urcli/wiki). Commands:

+ [setup](https://github.com/trolster/urcli/wiki/setup)
+ [assign](https://github.com/trolster/urcli/wiki/assign)
+ [token](https://github.com/trolster/urcli/wiki/token)
+ [revenue](https://github.com/trolster/urcli/wiki/revenue)
+ [certs](https://github.com/trolster/urcli/wiki/certs)

## The configuration file

The `setup` command creates a configuration folder in your home folder. You find the configuration file here `~/.urcli/config.json`.

## Contributing

Got a question or an idea? Found a bug? Check out our [contributing guidelines](https://github.com/trolster/urcli/blob/master/.github/CONTRIBUTING.md) for ways to offer feedback and contribute.

For very minor changes:

1. Fork this repository
1. Create your branch (`git checkout -b my-new-thing`)
1. Commit your changes (`git commit -am 'commit-message'`)
1. Push to the branch (`git push origin my-new-thing`)
1. Create a new Pull Request

For new features you need to do everything above, but before you write any code you should first read the [contributing guidelines](https://github.com/trolster/urcli/blob/master/.github/CONTRIBUTING.md) and then open an issue explaining what you have in mind. Making sure your feature fits with the direction the project is going can save you a lot of otherwise wasted effort.

## License

[MIT](LICENSE) © Mikkel Trolle Larsen.
