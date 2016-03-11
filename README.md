Joomla! Framework

Build Status

What is the Joomla! Framework ?

The  Joomla! Framework  is a platform for writing web and command line applications in PHP. It is free and open source software, distributed under the GNU General Public License version 2 or later.

It is composed of code originally developed for the Joomla Content Management System (CMS). For more information about the Joomla CMS visit http://www.joomla.org/about-joomla.html.

For news and information about developing with Joomla, please visit http://developer.joomla.org.

View the Joomla Framework API Documentation at http://api.joomla.org and is powered by phpDocumentor 2.

You can discuss Joomla Framework development by joining the mailing list at http://groups.google.com/group/joomla-dev-framework.

Requirements
•PHP 5.3.10
•Each package has their own requirements as well. Ex: The Image package requires the PHP GD extension. Please see the  composer.json  in each package repository for these requirements.
•Applications implementing the Joomla Framework must implement the 'JPATH_ROOT' constant which should be the root path of the application.

Installation

The simplest way to get up and running with the Joomla Framework is to use composer. Basic installation for composer can be found below, for additional information on installing composer, read the documentation.

curl -sS https://getcomposer.org/installer | php

Full Installation Via Composer

Composer has the ability to download the full stack framework (including all our packages) as a project starter using the "create-project" command. In the example below, "myAwesomeApp" is the folder where you want to create the project. It should not be created yet.

php composer.phar create-project --prefer-dist joomla/framework myAwesomeApp

If you are interested in working with the development code (in the master branch), and not a tagged stable distribution, then pass in the  --stability="dev"  command after  --prefer-dist .

Package Installation Via Composer

There are two ways to add our packages to your existing composer powered application.

Adding packages manually to the  require  option in your  composer.json .

{
    "require": {
        "joomla/PACKAGENAME": "VERSION"
    }
}

and then run install (or update).

php composer.phar install

Adding packages using  composer require 

php composer.phar require joomla/packagename:version

Full Installation Via Git

 git clone git://github.com/joomla/joomla-framework.git 

Documentation

General documentation about the Joomla Framework can be found under the /docs folder of this repository. In addition, each package has documentation in a  README.md  file.

Reporting Bugs and Issue

Bugs and issues found in the Joomla Framework code can be reported on the Issues list. Even for distributed packages where the code is in another repo, please submit issues to this issue tracker.

Contributing

All kind of contributions are welcome. Please read about how to contribute here.

You may find tasks you can do on the Issues list by filtering on labels and milestones

