## Mobile :-

1.Install necessary packages.

### `pkg install openssh nmap -y`

2. Run the ssh server

### `sshd`

3. Copy your username 

### `whoami`

**u0_a118**

4. Set a password for user

### `passwd u0_a118`

5. Find your local IP Address

### `ifconfig wlan0` 0r `ifconfig`

**192.168.43.1**

6.  find your ssh port number ( Mostly it will be 8022).

### `nmap localhost`

**8022**


## Terminal : -

7. Type the command to connect your termux with your Terminal

> ssh username@your-Ip-address -p portnumber

Examaple : 

```bash
ssh u0_a118@192.168.43.1 -p 8022

```

After you type the correct command and press enter you will see an in the last line it says that "are you sure you wanna continue connecting" Just **type Yes** press Enter. 

And Now you have t**o type your password that you used while setup,** **type that password and Press Enter and you will be inside your Termux Terminal**


### Clone Obsidian Vault : -

1. Change Directory to Document Folder

```bash
cd /storage/emulated/0/Documents
```

2. Git clone obsidian repository (SSH)

```bash
git clone git@github.com:plr7edu/obsidian-vaults.git

```

## How to Close the SSH server in Termux?

**To close the ssh serve you can always close or exit your termux** and the ssh server will automatically be turned off but if you don't wanna close your termux then **you can kill the ssh process using the below command.**

### `pkill ssh`
