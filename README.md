# autoreboot
Autoreboot script, run from cron

## Run daily - Daily at 06:05

5 6 * * * root /path/to/autoreboot

## Run daily weekdays - Daily weekdays at 06:05

5 6 * * 1-5 root /path/to/autoreboot

## Run once per week - Weekly on Monday at 06:05

5 6 * * 1 root /path/to/autoreboot

## Run one day per month - First Monday of each month at 06:05

5 6 1-7 * * root [ "$(date '+\%u')" = "1" ] && /path/to/autoreboot
