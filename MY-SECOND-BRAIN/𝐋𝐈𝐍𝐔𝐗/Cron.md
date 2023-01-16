
# What is Cron ?

- _cron_ is the time-based job scheduler in Unix-like computer operating systems. cron enables users to schedule jobs (commands or shell scripts) to run periodically at certain times, dates or intervals. It is commonly used to automate system maintenance or administration.

## Basic Commands : -

1. list all cron jobs 

### ```crontab -l

2. Create a cron job

### ```crontab -e```


To edit somebody else's crontab, issue the following command as root : -

### ``` # crontab -u _username_ -e  ```


## Crontab format : -

The basic format for a crontab is:

##### ```_minute_ _hour_ _day_of_month_ _month_ _day_of_week_ _command_```

![[crontab-layout.webp]]

-   _minute_ values can be from 0 to 59.
-   _hour_ values can be from 0 to 23.
-   _day_of_month_ values can be from 1 to 31.
-   _month_ values can be from 1 to 12.
-   _day_of_week_ values can be from 0 to 6, with 0 denoting Sunday.

Spaces are used to separate fields. To fine-tune your schedule you may also use one of the following symbols:

| Symbol | Description                                                |
| ------ | ---------------------------------------------------------- |
| **\*** | Wildcard, specifies every possible time interval           |
| **,**  | List multiple values separated by a comma.                 |
| **\-** | Specify a range between two numbers, separated by a hyphen |
| **/**  | Specify a periodicity/frequency using a slash              |

For example, the line:

##### ``*/5 9-16 * 1-5,9-12 1-5 ~/bin/i_love_cron.sh

- will execute the script `i_love_cron.sh` at five minute intervals from 9 AM to 4:55 PM on weekdays except during the months of June, July, and August.

- In addition, crontab has some special keywords :-

| Keyword       | Description          |
| ------------- | -------------------- |
| **@reboot**   | at startup           |
| **@yearly**   | once a year          |
| **@annually** | identical to @yearly |
| **@monthly**  | once a month         |
| **@weekly**   | once a week          |
| **@daily**    | once a day           |
| **@midnight** | identical to @daily  |
| **@hourly**   | once an hour         |

For example:

#### ```@reboot ~/bin/i_love_cron.sh```

- will execute the script `i_love_cron.sh` at startup.