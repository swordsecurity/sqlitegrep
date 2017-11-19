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
[*] Scanning table...contacts
[*] Discovered 3 matches.
(u'password', u'messages', u'the password is [hidden]')
(u'password', u'message', u'send me the password')
(u'email', u'contacts', u'john@doe.me')
```

