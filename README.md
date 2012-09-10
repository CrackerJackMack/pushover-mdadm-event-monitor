pushover-mdadm-event-monitor
============================

mdadm events for pushover.net


Install
=======

1. Copy mdadm-pushover somewhere accessible by mdadm daemon (/usr/local/sbin)
2. Edit the script placing your APIKEY with the appropriate value from the pushover dashboard
3. Make it as root executeable/readable chmod 400 mdadm-pushover (you won't want users running this)
4. Add the following to /etc/mdadm.conf:
        PROGRAM /usr/local/sbin/mdadm-pushover
5. restart/enable mdadm --monitor daemon
