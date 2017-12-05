
[Theme_HowTo](https://raw.githubusercontent.com/ogkarthik/references/master/theme_howto.md)

### To check different connection count from NETSTAT command
```
$ netstat -nap | awk '/tcp/ {print $6}'| sort | uniq -c

     27 CLOSE_WAIT
      1 CLOSING
   2583 ESTABLISHED
     15 FIN_WAIT1
      9 FIN_WAIT2
      6 LAST_ACK
     13 LISTEN
      6 SYN_RECV
   7485 TIME_WAIT
```
