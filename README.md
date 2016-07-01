# security-training

## Tools
- [Burp Suite](https://portswigger.net/burp/)
- [dirb](http://dirb.sourceforge.net/about.html) - Web Content Scanner
- [sqlmap](http://sqlmap.org/) - Automatic SQL injection and database takeover tool


## Web Content Scanner tools
### dirb
```dirb [url_base] [world_list_file]```

## SQL injections attacks
### Basic sniff
```sqlmap -u http://hostname:port```

### Time-based sniff
```sqlmap -u http://hostname:port/index.php?title=lorem --technique=T```

### Get database tables
```sqlmap -u http://hostname:port --tables```

### Dump table data
```sqlmap -u http://hostname:port --dump -t [table] --threads 10```
