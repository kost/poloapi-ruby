# Poloniex

[![Gem Version](https://badge.fury.io/rb/poloapi.png)](http://badge.fury.io/rb/poloapi)

This gem provides a ruby wrapper to the poloniex.com api: [Link](https://poloniex.com/api)
## Installation

Add this line to your application's Gemfile:

    gem 'poloapi'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install poloapi

## Usage

All methods provided by ```Poloapi``` are class methods, and are of the same name as the api ( except that "return"s have been removed ).

For example, ```https://www.poloniex.com/public?command=returnTicker``` is written as ```Poloapi.ticker```

The Poloapi module accepts a setup block for configuration:

```
Poloapi.setup do | config |
    config.key = 'my api key'
    config.secret = 'my secret token'
end
```

GET requests ( to /public ) do not need authentication, and therefor do not need Poloniex to be configured.

POST requests ( to /tradingApi ) will need authentication, and you will have to have your own key and secret token.



## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Credits

based on poloniex ruby gem available at: https://github.com/Lowest0ne/poloniex
