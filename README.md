![Screenshot](/screenshot.png?raw=true)

[Joomlatools Console]
=====================

This is a script developed by [Joomlatools](http://joomlatools.com) to ease the management of Joomla sites. It is designed to work on Linux and MacOS. Windows users can use it in [Joomlatools Vagrant box](https://github.com/joomlatools/joomla-vagrant)

Installation
------------

1. Install using Composer:

 `$ composer global require joomlatools/console`

1. Tell your system where to find the executable by adding the composer directory to your PATH. Add the following line to your shell configuration file called either .profile, .bash_profile, .bash_aliases, or .bashrc. This file is located in your home folder.

 `$ export PATH="$PATH:~/.composer/vendor/bin"`

1. Verify the installation

 `$ joomla --version`

1. To create a new site with the latest Joomla version, run:

  ```shell
     joomla site:create testsite
  ```

   The newly installed site will be available at /var/www/testsite and testsite.dev after that. The default Super User's name and password is set to: `admin` / `admin`.

   By default, the web server root is set to _/var/www_. You can pass _--www=/my/server/path_ to commands for custom values. You can choose the Joomla version or the sample data to be installed:

   ```shell
     joomla site:create testsite --joomla=2.5 --sample-data=blog
   ```

1. For other available options, run:

  `$ joomla --list`

1. Read our [documentation pages](http://developer.joomlatools.com/tools/console/usage.html) to learn more about using the tool.

## Requirements

* Composer
* Joomla version 2.5 and up.

## Contributing

Joomlatools Console is an open source, community-driven project. Contributions are welcome from everyone.
We have [contributing guidelines](CONTRIBUTING.md) to help you get started.

## Contributors

See the list of [contributors](https://github.com/joomlatools/joomlatools-console/contributors).

## License

Joomlatools Console is free and open-source software licensed under the [MPLv2 license](LICENSE.txt).

## Community

Keep track of development and community news.

* Follow [@joomlatoolsdev on Twitter](https://twitter.com/joomlatoolsdev)
* Join [joomlatools/dev on Gitter](http://gitter.im/joomlatools/dev)
* Read the [Joomlatools Developer Blog](http://developer.joomlatools.com/blog/)
* Subscribe to the [Joomlatools Developer Newsletter](http://developer.joomlatools.com/newsletter)

[Joomlatools Console]: http://developer.joomlatools.com/console
