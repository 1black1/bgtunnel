# Changelog

## 0.3.8 (2015-02-04)

* Make connection timeout handling better. Thanks to @howaryoo for the heads up in his PR
* Add support for setting the amount of connection attempts to make
* Fix Python 3 str/bytes exception that occurred when `Permanently added` warning was reported by the ssh command

## 0.3.7 (2014-08-07)

* Fixed typo in setup.py. Thanks to @soby for PR

## 0.3.6 (2014-04-16)

* Introduced a workaround for the connection validation expecting the server to write to stdout on a successful connection. Pass in `expect_hello=False` to `bgtunnel.open` to bypass the validation check. Thanks @hamiltont for the fix.

## 0.3.5 (2014-01-03)

* Fix AttributeError introduced in 0.3.4

## 0.3.4 (2014-01-03)

* Add identity_file option. Thanks to @kermit666

## 0.3.3 (2014-01-03)

* SIGTERM instead of SIGINT for background ssh process. Sometimes the process would not exit with SIGINT. Thanks to @fermayo

## 0.3.2 (2013-12-18)

* Use sudo for ssh command if a privileged host port was specified.

## 0.3.1 (2013-11-27)

* Notify before starting tunnel and once started

## 0.3.0 (2013-10-09)

* Raise exception on permission denied (password)
* Made ssh connectivity checking more robust

## 0.2.0 (2013-09-26)

* Added setup.py and registered to PyPI
* Basic testing with nose and tox
* Support for Python 2.6 and 3.3 in addition to 2.7
* Added a command for running bgtunnel directly from the terminal

## 0.1.1 (2013-09-19)

* No longer requires sh package

## 0.2.2 (2013-09-26)

* Made bgtunnel into a proper console script, installed on setup

## 0.1.0 (2013-09-13)

* Initial version
