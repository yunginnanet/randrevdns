# randrevdns

Small, fast, simple tool for performing reverse DNS lookups en masse (using random resolvers).

read files with targets and resolvers, it returns hostnames.

This can be a useful way of setting someone up the bomb.

## It might work if you do this maybe

```sh
git clone https://github.com/yunginnanet/randrevdns
cd randrevdns
echo "1.1.1.1" >> dnsResolvers.txt
echo "9.9.9.9" >> dnsResolver.txt
echo "198.251.80.62" >> targets.txt
echo "209.141.38.221" >> targets.txt
go run main.go
```


## Contributors
- [hakluke](https://twitter.com/hakluke) wrote the tool
- [alphakilo](https://github.com/Alphakilo/) added the option to use custom resolvers
- [SaveBreach](https://twitter.com/SaveBreach/) added the -d flag and cleaned up the code
- [yunginnanet](https://twitter.com/yunginnanet) massacred it and added resolver entropy
