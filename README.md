# geminabox
Gem in a Box PoC

## install

    gem install geminabox
    cd /path/to/geminabox
    mkdir data
    rackup # or unicorn or whatever

    cd /path/o/gems
    # upload ein gem
    gem inabox --host http://127.0.0.1:9292 ein_gem.gem

    # upload alle gems aus dem ordner
    for i in $(ls -1 *.gem); do echo $i; gem inabox --host http://127.0.0.1:9292 $i; done

## interface

auf http://127.0.0.1:9292/ kann man dann alle gems einsehen und auch noch welche hinzu laden.


## usage

### Gem Source

    $ gem sources --add http://127.0.0.1:9292

### Gemfile

    source "http://127.0.0.1:9292/"
    gem "private-gem"
