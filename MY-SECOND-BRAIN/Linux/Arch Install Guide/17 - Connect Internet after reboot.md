## Network Managers

![[2022-02-25_161658.png|700]]

## How to Connect to Wi-Fi Through the Linux Terminal With Nmcli

1. Check network status

### `nmcli dev status

![[Untitled picture.png]]

2. Check Wi-Fi device is enabled or not

### `nmcli radio wifi

![[Untitled picture1.png|500]]

If the output shows that the Wi-Fi is disabled, you can enable it with the following command :-

### `nmcli radio wifi on 

3. Identify a Wi-Fi Access Point

### `nmcli dev wifi list

![[Untitled picture2.png]]

4. Connect Wifi

### `sudo nmcli dev wifi connect network-ssid password "network-password"

![[Untitled picture3.png]]

### `sudo nmcli --ask dev wifi connect network-ssid

![[Untitled picture4.png]]

Ex =       

sudo nmcli dev wifi connect PLR_WIFI password "Appleboy"
sudo nmcli –ask dev wifi connect PLR_WIFI

5 .Test with a ping.

### `ping google.com

### <u>View all the saved connections</u>

### `nmcli con show

![[Untitled picture5.png]]


### <u>Disconnect the Internet Connections</u>

### `nmcli con down ssid/uuid

![[Untitled picture6.png]]

### <u>Connect another saved Internet connection</u>

### `nmcli con up ssid/uuid

[[18.1 - Activating Swap File]]
