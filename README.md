# Sqlitegrep
Use regular expressions to search in all the tables and columns of an SQLite database

# Usage
```
usage: sqlitegrep [-h] -d DATABASE -e EXPRESSION
```

# Example
```
./sqlitegrep -d corp.db -e '(password|email)'
[*] Scanning table...messages
[*] Discovered 3 matches.
(u'password', u'messages', u'the password is [hidden]')
(u'password', u'messages', u'send me the password')
(u'email', u'messages', u'my email is john@doe.me')
```

