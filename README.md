# python-env-tools
Script related to initiate python enviroment

## Install Script 
git clone git@github.com:wackoen/python-dev-tools.git

## python virtual environment (python 3.7 - only test for this version)
Create environment if not available
```console
user@server:~$ /usr/local/bin/python3 -m venv venv
```
Enable virtual environment
```console
user@server:~$ source venv/bin/activate
```

### Sqlite (if require)
```
   + sometime it easy to use lite version db such as sqlite (for testing)
   + if server/pc not provide (linux)
```

```console
user@server:~$ curl -O https://sqlite.org/2019/sqlite-autoconf-3300100.tar.gz
user@server:~$ tar xvzf sqlite-autoconf-3300100.tar.gz
user@server:~$ cd sqlite-*
user@server:~$ ./configure
user@server:~$ make
user@server:~$ make install
```
### Need to recompile python to enable sqlite extentions

```console
user@server:~$ cd /usr/src/Python-3.7.4/
user@server:~$ make clean
user@server:~$ ./configure --enable-optimizations --enable-loadable-sqlite-extensions
user@server:~$ make
user@server:~$ make install
```
