## Check Network Interfaces :-
### `ip addr show

![[2021-12-20_092524.png|1000]]

**enp0s3 = Ethernet (Wired Network Interface)**

## Connect WIFI

1. Iwctl ( Command for connect WIFI networks)
2. [iwd]# device list (Print a list of wireless interfaces)![[2021-12-20_094123.png]]

3.  (Find WIFI Access Points)

> station [Name of Wireless Device] scan

### `station wlan0 scan`

4.  (List WIFI networks that Found)

### `Station wlan0 get-networks

![[2021-12-20_095141.png]]

5. (Connect to the WIFI Network)

> station  [Device] connect "WIFI NAME"

### `station wlan0 connect "Atlantis"

![[2021-12-20_095838.png]]

6. (Check Network Connection)

Ping -c 5 8.8.8.8

**8.8.8.8 = Google DNS Server

![[2021-12-20_100234.png]]

[[4 - Update the system]]
