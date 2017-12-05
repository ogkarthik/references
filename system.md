[Theme_HowTo](https://raw.githubusercontent.com/ogkarthik/references/master/theme_howto.md)


### Calculate % of used ram memory
```
$ free | awk '/Mem/{printf("Used: %.2f%\n"), $3/$2*100} /buffers\/cache/{printf("Buffers: %.2f%\n"), $4/($3+$4)*100} /Swap/{printf("Swap: %.2f%\n"), $3/$2*100}'

Used: 98.62%
Buffers: 54.90%
Swap: 0.00%
```
