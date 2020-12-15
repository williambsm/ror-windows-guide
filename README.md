# How to Install Ruby on Rails for Windows
This is my own personal guide on how to set up Ruby on Rails on Windows. These are the steps that worked for me, and I hope that they will work for you as well!

Note: At any point where you check for install and it does not work, try restarting your computer before running the version check again.

## Install Ruby
1. Travel to this page: https://rubyinstaller.org/downloads/
2. Select the latest version of Ruby Devkit to the left side.
3. Download and run the installer.
4. Open a command line and type out "ruby -v" to verify that it was installed.

## Install Node.js
1. Travel to this page: https://nodejs.org/en/
2. Select the stable version of Node.js.
3. Download and install Node.js.
4. Open a command line and type out "node -v" to verify that it was installed.

## Install Yarn
1. Travel to this page: https://classic.yarnpkg.com/en/docs/install/#windows-stable
2. Download the version that is offered to you and install it.
3. Open a command line and type out "yarn --version" to verify that it was intalled.

## Install Rails
1. Open a command line, and type out "gem install rails"
2. In that same command line, type out "rails --version" to see if it is installed.

## Install Webpacker
1. Open a command line, and type out "rails webpacker:install"
2. I don't actually know how to verify that it's installed properly.

## Install PostgreSQL
1. Travel to this page: https://www.enterprisedb.com/downloads/postgres-postgresql-downloads
2. Download the latest Windows version and install it.
3. Remember the password you set here, as you will need it later.
3. Run pgAdmin 4, enter the password to authenticate.

## Create your project folder
1. Create a folder anywhere for where you want to store your ruby projects, keep in mind you will need to travel to this folder often using command line.
2. In that folder, run the command line "rails new [project-name] -d postgresql".
3. Update your databse.yml by uncommenting the following lines (username, password, server, port).
4. Update the username to "postgres"
5. Update all those informations to be accurate, and update development table login information properly using the user "postgres" and the password you picked.
6. Run "rails server"
7. Open a browser and go to localhost:3000

## Enjoy your server!
