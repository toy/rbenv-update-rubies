This [rbenv](http://rbenv.org/) plugin installs updated versions for installed rubies. After installation plugin will propose to uninstall outdated versions.

For 1.8 and 1.9 versions including ree three version parts will be taken into account otherwise two:

- `1.8.7-p374 => 1.8.7-p375`
- `1.9.2-p326 => 1.9.2-p330`
- `1.9.3-p547 => 1.9.3-p550`
- `2.1.0 => 2.1.4`

## Installation

This plugin uses `rbenv-whatis` and `ruby-build`, so first two clones are for them:

```sh
mkdir -p "$(rbenv root)"/plugins
git clone https://github.com/rkh/rbenv-whatis.git "$(rbenv root)"/plugins/rbenv-whatis
git clone https://github.com/sstephenson/ruby-build.git "$(rbenv root)"/plugins/ruby-build
git clone https://github.com/toy/rbenv-update-rubies.git "$(rbenv root)"/plugins/rbenv-update-rubies
```

## Usage

Update all:

```sh
rbenv update-rubies
```

Update specific versions:

```sh
rbenv update-rubies 1.9.3-p551 2.1.4
```
