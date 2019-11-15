Fork of https://github.com/yjh0502/ovpn_proxy to re-arrange params order because I got confused with "to" and "from".

## OpenVPN tcp-to-udp proxy

OpenVPN tcp-to-udp proxy, written in Golang.
The proxy listens to a specified TCP address and proxies connections to UDP-mode OpenVPN server.

### Example

`opvn_proxy -from "localhost:1194" -to "0.0.0.0:1234" -mtu 1500`

Will redirect from port 1194 which is the UDP OpenVPN to port 1234 in TCP.
"From" UDP "to" TCP.

## See also

- OpenVPN protocol spec: http://openvpn.net/index.php/open-source/documentation/security-overview.html
