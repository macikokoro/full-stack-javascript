# MongoDB

Install MongoDB with homebrew

Update homebrew's package database

`brew update`

Install MongoDB

`brew install mongodb`

To have launchd start mongodb at login:

`ln -sfv /usr/local/opt/mongodb/*.plist ~/Library/LaunchAgents`

Then load mongodb:

`launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mongodb.plist`

If you don't need launchtl just run:

`mongod --config /usr/local/etc/mongod.conf`

Create the data directory.

`mkdir -p /data/db`

In your project root directory

Run `mongo`

Select database `db`

Show databases `show dbs`

Switch to your database `use mydb`

Confirm `db`

Show collections `show collections`

Display documents `db.testData.find()`

If you want to run MongoDB on demand skip the autostart on login step. Once you create your project folder `mkdir` an empty db folder and open two tabs in your terminal.

Run:

`mongod --dbpath ~/data/db`

and in the other tab run:

`mongod`

`brew info mongodb` for reinstall instructions

