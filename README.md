# python-env-tools
Script related to initiate python enviroment

## Install Script 

## python virtual environment (python 3.7 - only test for this version)
Create environment if not available
```console
user@server:~$ /usr/local/bin/python3 -m venv venv
```
Enable virtual environment
```console
user@server:~$ source venv/bin/activate
```

### Sqlite 
```
   + for easy testing is easy to use lite version db such as sqlite
   + if server/pc not provide (linux)
```
curl -O https://sqlite.org/2019/sqlite-autoconf-3300100.tar.gz

```console
user@server:~$ curl -O https://sqlite.org/2019/sqlite-autoconf-3300100.tar.gz
```
