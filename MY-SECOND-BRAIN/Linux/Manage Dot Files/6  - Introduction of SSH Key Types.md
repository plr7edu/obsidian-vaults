- There are four types of SSH [key algorithms](https://www.ssh.com/ssh/keygen/) in the market ==RSA, DSA, ECDSA, ED25519.== The following are the differences between them.

| SSH Key Type | First published | Key Sizes       | Note                                                                                                                                                                                                                     |
| ------------ | --------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| RSA          | 1977            | 2,048 / 4,096   | An old algorithm.<br>Choosing a different algorithm may be advisable. <br>It is quite possible the RSA algorithm will become practically breakable in the foreseeable future.<br>All SSH clients support this algorithm. |
| DSA          | 1994            | 1024            | An old US government Digital Signature Algorithm.<br>DSA is now considered weak and was disabled in OpenSSH 7.0                                                                                                          |
| ECDSA        | 1999            | 256 / 384 / 521 | A new Digital Signature Algorithm standardized by the US government<br>This is probably a good algorithm for current applications.<br>Most SSH clients now support this algorithm.                                       |
|ed25519       | 2011            |                 | This is a new algorithm added in OpenSSH.<br>Support for it in clients is not yet universal.<br>OpenSSH 6.5 introduced   ED25519 SSH keys in 2014 and they should be available on most operating   systems.              |

## Recommendation of Generating SSH Key
1. 

> ssh-keygen -t ecdsa -b 521

2. 

> ssh-keygen -t ed25519



| Algorithm           | Public key     | Private key |
| ------------------- | -------------- | ----------- |
| ED25519 (Preferred) | id_ed25519.pub | id_ed25519  |
| ECDSA               | id_ecdsa.pub   | id_ecdsa    |


1. Generate Key Pair

> ssh-keygen -t ed25519

![[Untitled picture 2.png]]

![[Untitled picture1 2.png]]

2. Go gitlab & add ssh pub key.


> Preferences > SSH Keys > Add an ssh key

![[Github SSH.png]]

3. Git Clone Repository using SSH

![[GIT Clone.png]]


[[7 - Dotfiles Repository]]