# ProtonVPN-server-load

Alternative to checking https://protonvpn.com/vpn-servers everytime you want to connect to a ProtonVPN server

Uses the ProtonVPN API [here](https://api.protonmail.ch/vpn/logicals)

Servers are restricted based on your plan (free, basic, plus), which corresponds to the Tier value of each server. Tier 0 is free, Tier 1 is basic, Tier 2 is plus. This script looks for servers in both Tier 1 and 2, but you can easily edit it at lines 37 to 41

## Usage:

```py
>>> import vpn_servers as vpns
>>> vpns.find_a_server_in("JP")
JP#25: 6%
>>> vpns.find_a_server_in("CH") # Switzerland
CH#5: 15%
```

You can get the country codes [here](https://protonvpn.com/vpn-servers)
