# BarkSpy Site Source

This is the source for the barkspy website found at http://barkspy.com

## Jekyll

[Jekyll](http://jekyllrb.com/) is a static site generator in built with [Ruby on Rails](http://rubyonrails.org/). With this approach, you are able to build a high power build system, but have a low power, very stable webserver running a static site.

Updates must be done by a build system, from this source repository.

### Updating the site

First change into the source directory of the site, once in, update via

    jekyll build

A simple script would be

    rm -rf /var/src/barkspy && mkdir -p /var/src/ && \
    git clone git@github.com:mattrude/barkspy.git /var/src/barkspy -q && \
    jekyll build -s /var/src/barkspy -d /var/www/barkspy.com -q && \
    rm -rf /var/src/barkspy

## Installing Jekyll
Since Jekyll only needs to be installed on your build system. Below are a few quick how-to's how setting up your build system.

### Installing Ruby on Ubuntu
On Ubuntu 14.04 LTS, you first need ruby installed on your setup, we will also install the development kit.

    apt-get install git ruby ruby-dev ruby-dir

Next install the needed gems and Jekyll

    gem install rails
    gem install kramdown
    gem install therubyracer
    gem install jekyll
    gem install jekyll-sitemap
    gem install jekyll-less

Now you may use Jekyll to build the site, using the source provided in this repository.

### Installing Ruby on Windows
First start out by downloading the current production version of the [Ruby Installer](http://rubyinstaller.org/downloads/) for windows.

#### Installing the Ruby Development Kit
After installing Ruby via the [Ruby Installer](http://rubyinstaller.org/downloads/) talked about above, you must now download the Development Kit.

1. Download the Development Kit from http://rubyinstaller.org/downloads/
1. Extract the contact into a location easy accessible to your command prompt.
1. Open a command prompt, change into the directory that you extracted the content of the Development Kit to and run the command: `rake devkit sfx=1`.

### Installing Ruby on OSX

