#URI

```regex
/((?<scheme>https?|ftp):\/?\/?)?(?<auth>((?<userinfo>(?<username>[A-z0-9]+)(:(?<password>[A-z0-9]+))?)@)?(?<host>(?<subdomain>[A-z0-9]+).(?<domainname>(?<name>[A-z0-9-]+)(?<extension>(?<subtopdomain>\.[a-z]+)?(?<topdomain>\.[a-z]+)))(:(?<port>[0-9]+))?))(\/)?(?<path>((?<dir>[A-z0-9-_\.%,]+)\/)*(?<resource>(?<resourcename>[A-z0-9-_,]+(\.[A-z0-9]+)??)(?<resourceextension>\.[A-z0-9]+)?)?)?(\?(?<query>((\&)?(?<querycontent>(?<querykey>[A-z0-9]+)\=(?<queryvalue>[A-z0-9]+))??)+))?(#(?<fragment>[A-z0-9]+))?$/mg
```

### Tested uri

```
https://www.test.com.us
```
```
http://www.test.com
```
```
http://www.test.com/
```
```
ftp://www.test.com/file.txt
```
```
http://user:123@www.test.com.us:100/test/dir/index.xml.php?uid=0&mode=view#id1
```
