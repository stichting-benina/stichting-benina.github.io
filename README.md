# Website for Benina Foundation. See [https://www.benina.nl](https://www.benina.nl)

Website created using a fork of Methods. See: [https://github.com/18F/methods](https://methods.18f.gov)

## Install

You will need [Ruby](https://www.ruby-lang.org) ( > version 2.1.5 ). You may consider using a Ruby version manager such as [rbenv](https://github.com/sstephenson/rbenv) or [rvm](https://rvm.io/) to help ensure that Ruby version upgrades don’t mean all your [gems](https://rubygems.org/) will need to be rebuilt.

On OS X, you can use [Homebrew](http://brew.sh/) to install Ruby in `/usr/local/bin`, which may require you to update your `$PATH` environment variable:

```shell
brew update
brew install ruby
```

```
rbenv global 3.2.3
gem install bundler
gem install posix-spawn -- --with-cflags="-Wno-incompatible-function-pointer-types"
gem install bundler

```
To serve this website locally, using `website` as the name of your new repository:
Run each of the following steps to get the site up and running.

```shell
git clone https://github.com/stichting-benina/stichting-benina.github.io.git website
cd website
bundle install
bundle exec jekyll serve
```

You should be able to see the site at: `http://localhost:4000/`
