Fork of https://github.com/yjh0502/ovpn_proxy to add logs.

## OpenVPN tcp-to-udp proxy

OpenVPN tcp-to-udp proxy, written in Golang.
The proxy listens to a specified TCP address and proxies connections to UDP-mode OpenVPN server.

### Example

`opvn_proxy -from "0.0.0.0:1234" -to "localhost:1194" -mtu 1500`

Will redirect from port 1234 which is the client TCP connection, to the OpenVPN server on port 1194 in UDP.
"From" TCP "to" UDP.

## See also

- OpenVPN protocol spec: http://openvpn.net/index.php/open-source/documentation/security-overview.html
