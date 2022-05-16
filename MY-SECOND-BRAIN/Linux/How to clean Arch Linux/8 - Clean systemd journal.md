- Systemd stores its logs in /var/log/journal/ and these logs can be very useful.

1. Check for failed systemd services :-

### `sudo systemctl –failed

2. Second, check for errors in logfiles : - 

### `sudo journalctl -p 3 –xb

![[Untitled picture19 1.png|1000]]

3. You can clean these log files manually when you run out of space. You can keep only the latest logs by size limit (e.g. keep only 50Mb of the latest logs) :-

### `sudo journalctl --vacuum-size=50M

Or by time limit (e.g. last 4 weeks) :- 

### `sudo journalctl --vacuum-time=4weeks

4. You can also set such limit as permanent and never worry about cleaning the logs.

Just edit the file /etc/systemd/journald.conf by uncommenting SystemMaxUse= and setting the size limit :-

> SystemMaxUse=50M

