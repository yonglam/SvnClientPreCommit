# SvnClientPreCommit

Pre-commit check on svn client side.

Sometimes you need to add some test code in your local working copy, but you don't want to really commit it to the server side. This script will make sure that your test code will not be commited. Of course you can change it to do anything more.

##Feature:
* Prevent test code commiting to server

##Usage:
1. Copy `svnci` script to '/usr/local/bin'
* Add comment which contains `@test` before your test code, such as '// hard code for @test'
* Use `svnci` instead of `svn ci` to commit your code, such as `svnci -m 'bug fix'`