mysql-foreign-key-checker
=========================

Checks a mysql database for foreign keys pointing to missing records.


1. Create the `db.yml` file in the same directory as this script.

```
   host: 192.168.10.10
   port: 3306
   username: user
   password: pass
   database: db_name
```

2. run `ruby ./find-invalid-keys.rb`


Note: MacOS Catalina Install mysql2

```
$ gem install mysql2 -v '0.5.3' -- --with-cflags="-I/usr/local/opt/openssl/include" --with-ldflags="-L/usr/local/opt/openssl/lib"
```
