# Environment Setup

Get started with node, install the following tools:

Latest version of Ruby \(for Sass, and other tools\) Node.js, PostgreSQL, MongoDB, Redis,

Editors: [Atom.io](http://atom.io) or [Sublime Text](http://www.sublimetext.com/).

## Mac OS:

* Homebrew [http://brew.sh](http://brew.sh) Note: the instructions are at the end of the web page.
* rbenv, ruby-build, ruby 2.1.0 and the sass gem
  * `brew doctor`
  * `brew update`
  * `brew install rbenv ruby-build rbenv-gem-rehash`
  * `echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile`
  * `echo 'eval "$(rbenv init -)"' >> ~/.bash_profile`
  * `rbenv install 2.1.2`
  * `rbenv global 2.1.2`
  * `gem install sass`
  * Don't use sudo to install ruby or gems
  * If you get a permissions error when installing sass, somehow system ruby is still active. Try restarting your terminal, or if it persists, check for the items above in your .bash\_profile
* Node.js
  * `brew install nvm`
  * `nvm install 0.10`
  * `nvm alias default 0.10`
  * add `source $(brew --prefix nvm)/nvm.sh` to your .bash\_profile or .zshrc
  * Reference the [NVM README](https://github.com/creationix/nvm/blob/master/README.markdown) if you get stuck
* MongoDB
  * `brew install mongodb`
  * You may not want it to start at login, it's pretty easy to just run mongod when you need it.
  * Skip the instructions after the installation and create the db folder in your the root directory of you project. Then open a new terminal tab and run `mongod --dbpath ~/data/db` to start MongoDB.
  * After that open a second terminal tab and start MongoDB with `mongod`
* Heroku Toolbelt
  * `brew install heroku-toolbelt`
* Git
  * `brew install git` 
* Pick a programmer's editor:
  * [Atom.io](http://atom.io) is my personal favorite but a lot of developers choose Sublime Text 3:
    * [http://www.sublimetext.com/3](http://www.sublimetext.com/3)
    * Package Control: [https://sublime.wbond.net/installation](https://sublime.wbond.net/installation)

## Optional Installs until needed.

* Redis
  * brew install redis
  * same as above, you don't need it to start at login
* PostgreSQL
  * You can follow this [post](https://www.codefellows.org/blogs/how-to-install-postgresq) once you are ready.

## Ubuntu:

* No need for homebrew you already have a perfectly good [package management system](https://help.ubuntu.com/community/AptGet/Howto).
  * In your terminal preferences make sure that "Run Command as a login shell is an enabled profile preferences" check these two screenshots: [http://cl.ly/image/220M3f093v2M](http://cl.ly/image/220M3f093v2M) [http://cl.ly/image/3i2O0y0A3e04](http://cl.ly/image/3i2O0y0A3e04)
  * rbenv, ruby-build, and ruby: [https://www.digitalocean.com/community/articles/how-to-install-ruby-on-rails-on-ubuntu-12-04-lts-with-rbenv--2](https://www.digitalocean.com/community/articles/how-to-install-ruby-on-rails-on-ubuntu-12-04-lts-with-rbenv--2)
  * NOTE you DO NOT have to buy a digital ocean server, this is instructions for how to install LOCALLY. Ignore the create a server droplet step.
  * NOTE replace 1.9.3 with the latest version of ruby: 2.1.0
* gem install sass // DO NOT use sudo to install gems
* node.js: [https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)
* PostgreSQL
  * Follow this blog post: [https://www.codefellows.org/blogs/how-to-install-postgresql](https://www.codefellows.org/blogs/how-to-install-postgresql)
    * Sublime Text 3
  * [http://docs.sublimetext.info/en/latest/getting\_started/install.html](http://docs.sublimetext.info/en/latest/getting_started/install.html)
* MongoDB - [https://www.digitalocean.com/community/articles/how-to-install-mongodb-on-ubuntu-12-04](https://www.digitalocean.com/community/articles/how-to-install-mongodb-on-ubuntu-12-04)
  * NOTE you DO NOT have to buy a digital ocean server, these are instructions to install LOCALLY. Ignore the create a server droplet step.
  * Redis - [https://library.linode.com/databases/redis/ubuntu-12.04-precise-pangolin](https://library.linode.com/databases/redis/ubuntu-12.04-precise-pangolin) same as above
* Heroku Toolbelt - sudo apt-get install heroku-toolbelt

## Arch Linux and Manjaro

To set up your local dev follow this [tutorial](https://www.gitbook.com/book/jqn/installing-node-for-linux/details).

Here is another resource for installing ruby on rails:

[DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-on-arch-linux-with-rvm) how to install Ruby on Rails.

