# Calcurse Notifier

Simple bash script that sends notifications X minutes before events saved in calcurse. Will also send notifications X minutes before midnight for daily events.

Simply add something like the following to your crontab to enable. This line will notify you about events 30 minutes before they happen by running this script every two minutes.
```
*/2 * * * * export DBUS_SESSION_BUS_ADDRESS=unix:path=/run/user/$(id -u)/bus; /path/to/calendar_appointment_notify.sh 30 2
```
