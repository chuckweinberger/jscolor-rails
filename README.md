# jscolor-rails

A gem that makes [JSColor](http://jscolor.com/) available to the Rails asset pipeline.

## Installation

Add this line to your application's Gemfile:

    gem 'jscolor-rails'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jscolor-rails

## Usage

Add the following to any JavaScript file:

    //= require jscolor
    
### Asset path

One tweak has been applied to jscolor.js. `jscolor.dir`'s default value has been changed to `'/assets/'` because jscolor's auto-detect fails in production mode. To change the default, do the following:

````javascript
jscolor.dir = '/path/to/assets/';
````

## Versioning

The gem version number tracks JSColor's version number.

The major, minor, and patch version numbers will always represent the JSColor version. Should a gem bug be discovered, a 4th version identifier will be added and incremented.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
