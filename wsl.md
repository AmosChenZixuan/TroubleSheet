# Unable to resolve host in wsl 

networking - Bash on Ubuntu on Windows - could not resolve host using VPN - Super User 

``` 

Get-DnsClientServerAddress -AddressFamily IPv4 | Select-Object -ExpandPropert ServerAddresses 

``` 

Add results to /etc/resolv.conf as nameservers 