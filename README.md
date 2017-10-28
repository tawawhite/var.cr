# var.cr [![Build Status](https://travis-ci.org/maiha/var.cr.svg?branch=master)](https://travis-ci.org/maiha/var.cr)

`Object.var` macro for [Crystal](http://crystal-lang.org/).

- crystal: 0.24.0

## Usage

```crystal
class MyClass
  var foo : String
  var debug = false
end

my = MyClass.new
my.foo # raises Var::NotReady

my.foo = "ok"
my.foo # => "ok"

my.debug? # => false
```

## Installation

Add this to your application's `shard.yml`:

```yaml
dependencies:
  var:
    github: maiha/var.cr
    version: 0.2.1
```

Then require it in your app.
```crystal
require "var"
```

## Development

```shell
make test
```

## Contributing

1. Fork it ( https://github.com/maiha/var.cr/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [maiha](https://github.com/maiha) maiha - creator, maintainer
